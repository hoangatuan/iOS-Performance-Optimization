# iOS-Performance-Optimization
This project contains highly recommended resources on how you can optimize your iOS application performance

# Table of Contents

- [Reduce App Size](#reduce-app-size)
- [Reduce Build time](#reduce-build-time)
- [App Launch time](#App-launch-time)
- [App Runtime](#App-run-time)
- [App Hang](#App-hang)
- [Memory usage](#memory-usage)

## Reduce App Size

### Foundation knowledge

- [Understand iOS App Size](https://docs.emergetools.com/docs/ios-app-size) by Emerge
- [Understand static framework & dynamic framework](https://www.emergetools.com/blog/posts/static-vs-dynamic-frameworks-ios-discussion-chat-gpt) by Emerge
- [Basic optimization to reduce app size](https://developer.apple.com/documentation/xcode/doing-basic-optimization-to-reduce-your-app-s-size) by Apple
- [Advance optimization to reduce app size](https://developer.apple.com/documentation/xcode/doing-advanced-optimization-to-further-reduce-your-app-s-size) by Apple
- [Reducing app size](https://developer.apple.com/documentation/xcode/reducing-your-app-s-size) by Apple

### Tools

- [Emerge Tool size Analysis](https://www.emergetools.com/uploads)
- [Periphery - Unused code detection](https://github.com/peripheryapp/periphery)
- [FengNiao - Unused image detection](https://github.com/onevcat/FengNiao)

### Real-life example

- [How Uber Deals with Large iOS App Size](https://www.uber.com/en-SG/blog/how-uber-deals-with-large-ios-app-size/)
- [How 7 iOS Apps Could Save You 500MB of Storage](https://www.emergetools.com/blog/posts/7AppsThatCouldSaveYou500MB) by Emerge
- [Spotify](https://www.youtube.com/watch?v=v3rYaEXzRh4)
- [Make Your iOS App Smaller with Dynamic Frameworks](https://www.emergetools.com/blog/posts/make-your-ios-app-smaller-with-dynamic-frameworks)

## Reduce Build time

### Foundation knowledge

- [Clean build vs. Incremental build](https://emndeniz.medium.com/xcode-build-time-optimization-abee9893e4c8)
- [Swift Compiler Performance](https://github.com/apple/swift/blob/main/docs/CompilerPerformance.md) by Apple 

### Tools

- [Xcode Build time Rendering](https://github.com/PaulTaykalo/xcode-build-times-rendering)
- [XCMetrics](https://github.com/spotify/XCMetrics)
- [Tuist](https://github.com/tuist/tuist)
- Bazel

### Real-life example

- [Grab](https://trinhngocthuyen.com/posts/tech/a-tale-of-project-build-time/)
- [Gojek](https://medium.com/gojekengineering/reducing-our-build-time-by-50-835b54c99588)
- [Tokopedia](https://medium.com/tokopedia-engineering/how-tokopedia-achieved-1000-faster-ios-build-time-7664b2d8ae5)
- [Building faster](https://developer.apple.com/videos/play/wwdc2018/408) by Apple

## App launch time

### Foundation knowledge

- [About the app launch sequence](https://developer.apple.com/documentation/uikit/app_and_environment/responding_to_the_launch_of_your_app/about_the_app_launch_sequence) by Apple
- [Cold launch vs Warm launch](https://developer.apple.com/documentation/xcode/reducing-your-app-s-launch-time#Understanding-cold-and-warm-launch): Apple
- [Dynamic Linker vs Static Linker](https://developer.apple.com/library/archive/documentation/DeveloperTools/Conceptual/DynamicLibraries/100-Articles/OverviewOfDynamicLibraries.html)

### Tools

- Xcode Instruments

### Real-life example

- [Apple](https://developer.apple.com/documentation/xcode/reducing-your-app-s-launch-time)
- [Uber](https://www.uber.com/en-SG/blog/measuring-performance-for-ios-apps-at-uber-scale/?uclick_id=50770e44-6b39-4177-9e17-b24247f0b7f6)
- [Facebook Dynamic Loading](https://medium.com/@stevedao91/dynamic-loading-for-ios-6229d39a0a70)

## App Runtime

### Foundation Knowledge

### Tools

- [os signpost](https://www.donnywals.com/measuring-performance-with-os_signpost)

## App Hang

## Memory Usage
