# Changelog
All notable changes to this package will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [0.28.0] - 2020-07-27
### What's new
* Basic in-game text rendering support
* CPU/GPU mesh skinning 
* The ability to select the render graph properties at build or run time
* Dynamically assign lights
* Add WebP image lossy/lossless encoding
* Improve audio assets decompression on web
* Build web into a single HTML file export 
* Use .NET Core to run il2cpp on Windows and MacOS
* Improve IL2CPP code generation to make code size smaller
* Profiler multi-threading support
* PlayerConnection multi-threading support
* Android and iOS advanced build settings support
* Android ARM64 and FAT Support
* New build settings component to adjust allowed screen orientations

### Fixed
* Optimized the Tiny particles system
* Improve the tiny conversion workflow
* Clean up runtime memory usage on Android and iOS  
* Fixed an issue where audio volume may change with screen rotation on iOS
* Projection matrix is locked at 16:9 aspect ratio
* Web input can't distinguish between left and right keyboard control keys
* Audio may not properly play in web builds on iOS
* Improve Web build and run workflow
* Speed up building Android managed debugger targets
* DisplayInfo.ScreenDpiScale may return 0 on some platforms 
* Match the input position with the display info data
* PlayerConnection crashes on application shutdown when the application leaks memory 
* Textures do not load properly when managed debugging is enabled
* Fixed Emscripten WebGL/HTML5 API proxying for Offscreen Framebuffer
* Audio not working after minimizing and maximizing the app on iOS web builds
* Build and run web builds show raw html file
* Improve unsafe utility allocator for DOTS Runtime

## [0.27.0] - 2020-06-17
* Update package dependencies 

## [0.26.0] - 2020-05-26
### What's new
* Project Tiny Base Class Library: Added missing types basic collections (e.g. Dictionary, associated iterators) and System.IO.Stream. We’ve created a list of what’s included in the Project Tiny Base Class Library
* iOS: Modified iOS template project so it will use Storyboard for launch screen instead of XIB files
* Particles: Added support Start color and gravity modifier in particles system
Unity version: Project Tiny now requires Unity `2019.3.12f1` as a minimum supported version

### Fixed
* Android Input: GetMouseButtonUp/Down does not get triggered on android
* Audio is continues to play on iOS devices even if the silent button is turned on
* Texture V scale < 1 has wrong behavior
* iOS Wasm & AsmJS: No sound is playing
* Cannot build when specifying absolute path as output directory
* Depth sorting is not working

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
