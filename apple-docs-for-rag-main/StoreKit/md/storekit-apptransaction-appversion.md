

- StoreKit
- AppTransaction
-  appVersion 

Instance Property

# appVersion

The app version that the app transaction applies to.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let appVersion: String
```

## Discussion

This value is the version string you entered in Xcode. This value is a machine-readable string composed of one to three period-separated integers, such as `10.4.1`.

## See Also

### Getting app and version information

let bundleID: String

The bundle identifier that the app transaction applies to.

let originalAppVersion: String

The app version that the customer originally purchased from the App Store.

let appID: UInt64?

The unique identifier the App Store uses to identify the app.

let appVersionID: UInt64?

The number that the App Store uses to uniquely identify the version of the app.

