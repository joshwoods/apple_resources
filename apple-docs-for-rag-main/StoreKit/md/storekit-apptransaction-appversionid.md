

- StoreKit
- AppTransaction
-  appVersionID 

Instance Property

# appVersionID

The number that the App Store uses to uniquely identify the version of the app.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let appVersionID: UInt64?
```

## Discussion

The App Store assigns this value. In the sandbox and xcode environments, this value is `nil`.

## See Also

### Getting app and version information

let bundleID: String

The bundle identifier that the app transaction applies to.

let appVersion: String

The app version that the app transaction applies to.

let originalAppVersion: String

The app version that the customer originally purchased from the App Store.

let appID: UInt64?

The unique identifier the App Store uses to identify the app.

