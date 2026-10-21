# Known Issues
 
Last updated: 2026-10-21. Each issue names the game it affects. When an issue is fixed, it is removed from this list and the fix is listed in [CHANGELOG.md](CHANGELOG.md).
 
## RPCS3
 
**1. Freezes of about one second during races (Gran Turismo 6)**
- On RPCS3 v0.0.42-20037 and later, Gran Turismo 6 may freeze for about one second at a time during races, and the log reports "RSX queue appears to be stuck".
- This was introduced by "rsx: Fix USER_COMMAND behavior" (#19549) and has not been fixed upstream as of 2026-10-20.

**2. Vertex explosions with Multithreaded RSX (Gran Turismo 6)**
- With Multithreaded RSX enabled, Gran Turismo 6 may show black slivers and spikes on car bodies, for example in Gallery View, the garage, the Vision GT showroom and the purchase screen.
- RPCS3 copies some of the car's vertex data after the game has already replaced it. Turning Multithreaded RSX off resolves it.

**3. Motion blur flashes (Gran Turismo 6)**
- Gran Turismo 6 may show green or magenta flashes from the motion blur at Resolution Scale above 100% with Write Color Buffers and Read Color Buffers enabled.

**4. Crackling audio in the Bumper camera (Gran Turismo 6)**
- Gran Turismo 6 may have crackling audio in the Bumper camera with Disable ZCull Occlusion Queries enabled, as recommended by the RPCS3 wiki.
- Turning the setting off resolves the crackling, but car reward screens may slow down and updating car images in the Garage may softlock (see 5).

**5. Softlock when updating car images in the Garage (Gran Turismo 6)**
- With Disable ZCull Occlusion Queries turned off, Gran Turismo 6 may stop responding when updating more than a few car images in the Garage. This also happens without patches and on the official RPCS3 build.
- Turning Disable ZCull Occlusion Queries on resolves it. RPCS3 applies this setting while the game is running (in the game's custom configuration), so it can be turned on just for the update.
