# Changelog
All notable changes to this package will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [0.24.0] - 2020-04-14
### What's new
- Accelerometer/Gyro support for Android and iOS
- Screen orientation support on mobile
- Managed debugger support
- Support Unity profiler
- Pitch audio support
- Burst on iOS
- New particles system

### Fixed
- Support GUID assembly references in assembly definitions files
- If the Unity editor platform is changed, compilation errors show up in dots runtime code
- Memory leaks in Wasm builds
- InputSystem.GetInputDelta() always returns 0 in editor
- Re-init when default audio device changes
- Show error if sRGB sampling is not supported on Asmjs builds
- Fix lit transparent materials when fog enabled
- Game view is stretched when changing from portrait to landscape or vice versa during runtime

### Samples
- New Particles sample
- Add Motion sensors control to TinyRacing
- Add 3d audio and pitch-shifting to TinyRacing 


## [0.23.0] - 2020-03-21
* Update package dependencies

## [0.22.0] - 2020-02-21
* Update package dependencies

## [0.21.0] - 2020-02-06

* This is the first release of Unity.Tiny.All package.
