# iOS-Performance-Optimization
This project contains highly recommended resources on how you can optimize your iOS application performance

# Table of Contents

- [Reduce App Size](#reduce-app-size)
- [Reduce Build time](#reduce-build-time)
- [App Launch time](#App-launch-time)
- [App Runtime](#App-runtime)
- [App Hang](#App-hang)
- [Memory usage](#memory-usage)
- [CI](#ci)

## Reduce App Size

### Foundation knowledge

- [Understand iOS App Size](https://docs.emergetools.com/docs/ios-app-size) by Emerge
- [Understand static framework & dynamic framework](https://www.emergetools.com/blog/posts/static-vs-dynamic-frameworks-ios-discussion-chat-gpt) by Emerge
- [Basic optimization to reduce app size](https://developer.apple.com/documentation/xcode/doing-basic-optimization-to-reduce-your-app-s-size) by Apple
- [Advance optimization to reduce app size](https://developer.apple.com/documentation/xcode/doing-advanced-optimization-to-further-reduce-your-app-s-size) by Apple
- [Reducing app size](https://developer.apple.com/documentation/xcode/reducing-your-app-s-size) by Apple
- [Strip Binary Simple](https://docs.emergetools.com/docs/strip-binary-symbols)
- [Xcode build time optimization](https://tech.autoscout24.com/blog/posts/xcode-build-time-optimization/) 

### Tools

- [Emerge Tool size Analysis](https://www.emergetools.com/uploads)
- [Periphery - Static analysis - Unused code detection](https://github.com/peripheryapp/periphery) 
- [FengNiao - Unused image detection](https://github.com/onevcat/FengNiao)
- [Reaper by Emerge](https://docs.emergetools.com/docs/reaper): Dynamic analysis for Unused code

### Real-life example

- [How Uber Deals with Large iOS App Size](https://www.uber.com/en-SG/blog/how-uber-deals-with-large-ios-app-size/)
- [How 7 iOS Apps Could Save You 500MB of Storage](https://www.emergetools.com/blog/posts/7AppsThatCouldSaveYou500MB) by Emerge
- [Spotify](https://www.youtube.com/watch?v=v3rYaEXzRh4)
- [Make Your iOS App Smaller with Dynamic Frameworks](https://www.emergetools.com/blog/posts/make-your-ios-app-smaller-with-dynamic-frameworks)
- [Manage Image Resources](https://medium.com/p/45681f475461)
- [Duolingo remove 10000 lines of unused code by using Reaper](https://blog.duolingo.com/emerge-tools-reaper/)

## Reduce Build time

### Foundation knowledge

- [Clean build vs. Incremental build](https://emndeniz.medium.com/xcode-build-time-optimization-abee9893e4c8)
- [Swift Compiler Performance](https://github.com/apple/swift/blob/main/docs/CompilerPerformance.md) by Apple
- [Understanding Swift Performance](https://developer.apple.com/videos/play/wwdc2016/416/) by Apple: Understand how ARC works and how it impacts your app's performance
- [Performance of value type](https://swiftrocks.com/memory-management-and-performance-of-value-types) by Swiftrocks

### Tools

- [Xcode Build time Rendering](https://github.com/PaulTaykalo/xcode-build-times-rendering)
- [XCMetrics](https://github.com/spotify/XCMetrics)
- [Tuist](https://github.com/tuist/tuist)
- Bazel
- [Cocoapod binary cache](https://github.com/grab/cocoapods-binary-cache) by Grab
- [Build time analyzer](https://github.com/RobertGummesson/BuildTimeAnalyzer-for-Xcode): Measure the time Xcode takes to compile every funcs

### Real-life example

- [Grab](https://trinhngocthuyen.com/posts/tech/a-tale-of-project-build-time/)
- [Gojek](https://medium.com/gojekengineering/reducing-our-build-time-by-50-835b54c99588)
- [Tokopedia](https://medium.com/tokopedia-engineering/how-tokopedia-achieved-1000-faster-ios-build-time-7664b2d8ae5)
- [Building faster](https://developer.apple.com/videos/play/wwdc2018/408) by Apple
- [Caching SPM dependencies in CI](https://www.uptech.team/blog/swift-package-manager)

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
- [ETTrace](https://github.com/EmergeTools/ETTrace)

## App Hang

### Foundation Knowledge

- [Understanding hangs in your app](https://developer.apple.com/documentation/xcode/understanding-hangs-in-your-app)
- [Understand and eliminate hangs from your app](https://developer.apple.com/videos/play/wwdc2021/10258/)

### Tools

- [Track down hangs with Xcode and on-device detection](https://developer.apple.com/videos/play/wwdc2022/10082/): track hangs during pre-release testing, show you how to identify issues in release builds using the Xcode Organizer
- [Analyzing responsiveness issues in your shipping app](https://developer.apple.com/documentation/xcode/analyzing-responsiveness-issues-in-your-shipping-app)

## Memory Usage

### Foundation Knowledge

- [You don't always need weak self](https://medium.com/@almalehdev/you-dont-always-need-weak-self-a778bec505ef)
- [Nested closure weak self](https://medium.com/@almalehdev/the-nested-closure-trap-356a0145b6d)
- [Detect Unused code using Memory graph debugger](https://careers.doordash.com/blog/ios-memory-leaks-and-retain-cycle-detection-using-xcodes-memory-graph-debugger/)
- [Automating Memory Leak Detection with CI Integration](https://medium.com/gitconnected/automating-memory-leak-detection-with-ci-integration-for-ios-380f08a55f0b)

### Tools 

- [Memory Leaks Check](https://github.com/hoangatuan/MemoryLeaksCheck): A tool for detecting memory leak in CI

### Real life examples

- [The Memory Leak: An Xcode Detective Story by Emerge](https://www.emergetools.com/blog/posts/the-memory-leak-an-xcode-detective-story?utm_campaign%3DiOS%20CI%20Newsletter%26utm_medium%3Dweb%26utm_source%3DiOS%20CI%20Newsletter%20Issue%2051%26utm_content%3Dsep_23_24)

## CI

### Examples

- [Performance testing on CI](https://testableapple.com/xctmetric/?issue=043&utm_source=fatbobman%20weekly%20issue%2043&utm_medium=email&utm_campaign=fatbobman%20weekly)


