Simple Swift iOS project with RAC added via CocoaPods. It's not difficult to build this manually. I'm just putting this here to get examples up quickly.

## How to run this

Just clone me, then open the SwiftSlate/SwiftSlate.xcworkspace in Xcode (the latest Xcode 6 beta please).

## Do it yourself

This is what you have to do if you want to build something like this from scratch. I'm just putting this here in case you want to learn how I did this.

Things I did:
- Create a new Swift project
- Add gitignore to new Swift project
- Add Podfile with ReactiveCocoa in it
- Run `pod install`
- Add a bridging header file (see below)

Bridging Header:
- Create ReactiveSwift-Bridging-Header.h and add this: `#import <ReactiveCocoa/ReactiveCocoa.h>` (from: [@stigi](https://medium.com/@stigi/swift-cocoapods-da09d8ba6dd2x)'s post)
- TL;DR - Under the target's "Build Settings > Swift Compiler - Code Generation" section, update the "Objective-C Bridging Header" setting to: YOUR_APP_NAME/ReactiveSwift-Bridging-Header.h

