

- Bundle Resources
- Information Property List
-  LSMinimumSystemVersionByArchitecture 

Property List Key

# LSMinimumSystemVersionByArchitecture

The minimum version of macOS required for the app to run on a set of architectures.

macOS 10.0+

## Details 

Name  
Minimum system versions, per-architecture

Type  

object

## Properties

`i386`

`string`

Default: `10.0.0`

`ppc`

`string`

Default: `10.0.0`

`ppc64`

`string`

Default: `10.0.0`

`x86_64`

`string`

Default: `10.0.0`

## Discussion

The possible dictionary keys are: `i386`, `ppc`, `ppc64`, and `x86_64`. The values are the minimum version for the architecture. The default values are `10.0.0`.

## See Also

### Operating system version

LSMinimumSystemVersion

The minimum version of the operating system required for the app to run in macOS.

**Name:** Minimum system version

MinimumOSVersion

The minimum version of the operating system required for the app to run in iOS, iPadOS, tvOS, and watchOS.

LSRequiresIPhoneOS

A Boolean value indicating whether the app must run in iOS.

**Name:** Application requires iPhone environment

WKApplication

WKWatchKitApp

A Boolean value that indicates whether the bundle is a watchOS app.

