# Changelog
All notable changes to this package will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [0.25.0] - 2020-04-30
### What's new
* Multi-touch on Android and iOS
* Mouse wheel input support
* Particles billboard support 
* Ability to change the rendering borders background-color
* Support unity.physics 0.3.2-preview 
* Burst support on Android builds
* New generate Dots solution window
* Support build and run web builds in the browser
* Web player connection support for profiler & debug information

### Fixed
* Improve rendering performance on web builds 
* Web builds will no longer play audio if the browser is in background
* Fix potential memory leak on il2cpp builds
* Spaces in the build configuration name cause build failures
* Web on iOS: Touch is not removed from Touches after minimizing the browser
* Models with a large number of vertices cause Uint16 overflow exception during conversion
* Auto-select graphics backend for Web
* Optimize texture initialization loop at startup for WebGL targets
* Remove redundant glEnable/DisableVertexAttribArray calls
* Fixed issue where input coordinates are not scaled for HDPI
* Remove the requirement for including Rendering.Hybrid assembly in filter settings


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
