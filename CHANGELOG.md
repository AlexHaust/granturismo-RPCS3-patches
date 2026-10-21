# Changelog - 20261014

## New Patches

**1. Gran Turismo 5 (2.11, US and EU)**

- Aspect Ratio (with a 48:9 option)
- Extended FOV
- Camera Rotation in Chase View
- Camera Rotation in Roof/Hood View

**2. Gran Turismo 6 (1.22 and 1.05)**

- Disable Depth of Field
- Accurate Throttle Linearity
- Analog Dials in All Cameras
- Analog Dials in Roof Camera
- Camera Rotation in Chase View
- Camera Rotation in Roof/Hood View
- Lamp Glare Intensity
- Enable Motion Blur in Gameplay - 16 Samples
- Enable Motion Blur in Gameplay - 24 Samples
- Use Sharper MLAA
- Use Sharper MLAA - Strong
- Use Sharper MLAA - Custom
- Bloom/Glare Resolution Scale Fix
- Auto Exposure Resolution Scale Fix
- Sharper Shadows
- Sharper Shadows - 2x Filter Samples
- Sharper Shadows - 4x Filter Samples
- Sharper Shadows - 8x Filter Samples

## Improvements and Fixes

**1. Disable Driver Rendering**
- Car parts such as doors, bumpers, hoods, wipers and tachometer needles are no longer removed along with the driver (Gran Turismo 5 and Gran Turismo 6).
- Car audio such as engine, exhaust and tire noise is no longer affected (Gran Turismo 6 1.05).

**2. Disable Steering Wheel Rendering**
- Car parts such as doors, bumpers, hoods, wipers and tachometer needles are no longer removed along with the steering wheel (Gran Turismo 5 and Gran Turismo 6).

**3. Disable MLAA (Gran Turismo 6)**
- "Disable SPU MLAA" has been renamed "Disable MLAA".
- Bloom/glare is now kept when MLAA is disabled.

**4. Enable Bloom/Glare in All Cameras (Gran Turismo 6)**
- Can now be used together with Disable MLAA.

**5. Extended FOV (Gran Turismo 6)**
- The vertical FOV can now be set separately for the Bumper, Cockpit, Roof/Hood and Chase cameras, in degrees.

**6. Enable Motion Blur in Gameplay (Gran Turismo 6)**
- A Shutter Rate setting has been added to adjust the length of the blur.
- Motion blur is now enabled only in the Bumper, Cockpit, Roof/Hood and Chase cameras instead of in every scene the game renders.
- An issue where 3D menus showed the previously visited screen in the background has been resolved.
- An issue where the flag animation and venue logo before the pre-race menu were replaced by the previously visited screen or a black screen has been resolved.
- An issue where motion blur caused stuttering, audio crackling and frame rate drops at high Resolution Scale settings has been resolved.
- An issue where the car left a trailing afterimage in the Chase camera has been resolved.

**7. Patch Groups**
- The following patches can no longer be enabled at the same time as other patches in their group:
  - Analog Dials in All Cameras and Analog Dials in Roof Camera

**8. Others**
- Patch Version has been set to 1.0 for all patches, except Aspect Ratio (Gran Turismo 5), which is 1.1.
- Notes have been revised for most patches.
- Comments describing each patch line have been added to most patches.
- Author credits have been corrected for Disable Motion Blur and Develop Settings.
- Unused anchors have been removed.
- The Aspect Ratio options for Gran Turismo 6 have been reduced to single-monitor ratios plus 32:9 and 48:9.
- illusion's original Disable Motion Blur and Disable Anti Aliasing patches have been added for Gran Turismo 6 (BCUS99247).

## Known Issues

**1. RPCS3**
- On RPCS3 v0.0.42-20037 and later, Gran Turismo 6 may freeze for about one second at a time during races, and the log reports "RSX queue appears to be stuck". This was introduced by "rsx: Fix USER_COMMAND behavior" (#19549) and has not been fixed upstream as of 2026-10-14.
- Gran Turismo 6 may show green or magenta flashes from the motion blur at Resolution Scale above 100% with Write Color Buffers and Read Color Buffers enabled.
- Gran Turismo 6 may have crackling audio in the Bumper camera with Disable ZCull Occlusion Queries enabled, as recommended by the RPCS3 wiki. Turning the setting off resolves the crackling, but car reward screens may slow down.
