

- Bundle Resources
- Information Property List
-  LSMinimumSystemVersion 

Property List Key

# LSMinimumSystemVersion

The minimum version of the operating system required for the app to run in macOS.

Mac Catalyst 13.0+macOS 10.0+

## Details 

Name  
Minimum system version

Type  

string

## Attributes 

Default: `10.0.0`

## Discussion

Use this key to indicate the minimum macOS release that your app supports. The App Store uses this key to indicate the macOS releases on which your app can run, and to show compatibility with a person’s Mac.

Starting with macOS 11.4, the lowest version number you can specify as the value for the LSMinimumSystemVersion key is:

- `10` if your app links against the macOS SDK.

- `10.15` if your app links against the iOS 14.3 SDK (or later) and builds using Mac Catalyst.

- `11` if your iPad or iPhone app links against the iOS 14.3 SDK (or later) and can run on a Mac with Apple silicon.

To specify the minimum version of iOS, iPadOS, tvOS, or watchOS that your app supports, use MinimumOSVersion.

## See Also

### Operating system version

LSMinimumSystemVersionByArchitecture

The minimum version of macOS required for the app to run on a set of architectures.

**Name:** Minimum system versions, per-architecture

MinimumOSVersion

The minimum version of the operating system required for the app to run in iOS, iPadOS, tvOS, and watchOS.

LSRequiresIPhoneOS

A Boolean value indicating whether the app must run in iOS.

**Name:** Application requires iPhone environment

WKApplication

WKWatchKitApp

A Boolean value that indicates whether the bundle is a watchOS app.

