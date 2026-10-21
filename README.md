# granturismo5-6-patches
RPCS3 patches for Gran Turismo 5 and 6: camera, graphics, HUD and control tweaks.
 
All patches are in `imported_patch.yml`; see Installation below.
 
# Supported Games
| Game | Version | Serials |
|---|---|---|
| Gran Turismo 5 | 2.11 | BCUS98114 (US), BCES00569 (EU) |
| Gran Turismo 6 | 1.22 | BCUS98296 (US), BCES01893 (EU), BCES01977 (UK) |
| Gran Turismo 6 | 1.05 | BCUS98296 (US), BCES01893 (EU), BCES01977 (UK) |
 
# ⚠️ Warning! ⚠️
**Do not modify `imported_patch.yml`**, for example by copying entries under another PPU executable hash so that they show up for your serial in the Patch Manager. The patches are only made for the versions and serials listed under Supported Games, and RPCS3 skips an entry when another patch file has one with the same name and an equal or higher Patch Version, so an edited file can leave some patches without effect. **Support for the other regions is planned; until your serial is listed, please wait for an update instead of editing the file.**
 
**The patches are for RPCS3 only. It is not advised to use them on a real PS3, for example by converting them into Artemis PS3 codes.** Many entries rely on features only RPCS3's patch system has, such as extra memory for added code, so a converted code can freeze or crash the game. They are also made and tested only on RPCS3. Real PS3 setups are not supported at this time. Testing with Artemis PS3 is welcome, however; please share your results, including the game's serial and version and the entries you converted.
 
# Installation
1. Make sure the game is on a version listed under Supported Games; the game list's **Version** column shows the installed version.
2. Copy `imported_patch.yml`, unchanged, into RPCS3's `patches` folder (create the folder if it doesn't exist):
   - Windows: the `patches` folder next to `rpcs3.exe`
   - Linux: `~/.config/rpcs3/patches/` (Flatpak: `~/.var/app/net.rpcs3.RPCS3/config/rpcs3/patches/`)
   - macOS: `~/Library/Application Support/rpcs3/patches/`
   
   Keep the name `imported_patch.yml`. Don't rename it to `patch.yml`: that is RPCS3's own patch list, which RPCS3 replaces when it downloads the latest patches. If the folder already has an `imported_patch.yml` with patches from elsewhere, keep a copy of it, because the new file replaces them.
3. In RPCS3, open **Manage > Game Patches**, or right-click the game and choose **Manage Game Patches**.
4. Open **Gran Turismo 6** (or **Gran Turismo 5**), then your serial and version, for example **BCUS98296 v.01.22**, and tick the patches you want. Some patches have options under **Configurable Values**.
5. Click **Save**, then start the game. Patches are applied when the game starts, so restart it if it's already running.
To check that a patch is active, look for `Applied patch` lines in RPCS3's log.
 
## Updating
Replace `imported_patch.yml` with the new file. **Don't drag the new file onto the Patch Manager to import it**: the import skips entries whose Patch Version is not higher than the one already installed. Ticked patches and their values are kept, unless a patch is renamed.

# Reporting Issues
Please report any issue you run into. A new issue must include:
- The game's serial and version, for example BCUS98296 1.22.
- The RPCS3 version or build, as shown in RPCS3's title bar, for example 0.0.38-18345.
- The RPCS3 log file (`RPCS3.log`) from the session in which the issue happened. Save it before starting RPCS3 again, because RPCS3 replaces it on every start.
- Both patch files from RPCS3's `patches` folder: `imported_patch.yml` and `patch.yml`.
- The entries that were ticked in the Patch Manager.

For Artemis PS3 results, include the game's serial and version, the entries you converted, and what happened, instead of the RPCS3 log and patch files.
 
**Issues that do not include all of this information will be ignored and/or closed.**


TODO: patch list, usage notes, credits, roadmap
