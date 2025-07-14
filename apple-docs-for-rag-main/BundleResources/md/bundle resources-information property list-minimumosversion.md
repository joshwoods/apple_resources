

- Bundle Resources
- Information Property List
-  MinimumOSVersion 

Property List Key

# MinimumOSVersion

The minimum version of the operating system required for the app to run in iOS, iPadOS, tvOS, and watchOS.

iOS 3.0+iPadOS 3.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

## Details 

Type  

string

## Mentioned in 

Managing Your App’s Information Property List

## Discussion

The App Store uses this key to indicate the OS releases on which your app can run.

Don’t specify `MinimumOSVersion` in the `Info.plist` file for apps built in Xcode. It uses the value of the Deployment Target in the General settings pane.

For macOS, see LSMinimumSystemVersion.

## See Also

### Operating system version

LSMinimumSystemVersion

The minimum version of the operating system required for the app to run in macOS.

**Name:** Minimum system version

LSMinimumSystemVersionByArchitecture

The minimum version of macOS required for the app to run on a set of architectures.

**Name:** Minimum system versions, per-architecture

LSRequiresIPhoneOS

A Boolean value indicating whether the app must run in iOS.

**Name:** Application requires iPhone environment

WKApplication

WKWatchKitApp

A Boolean value that indicates whether the bundle is a watchOS app.

