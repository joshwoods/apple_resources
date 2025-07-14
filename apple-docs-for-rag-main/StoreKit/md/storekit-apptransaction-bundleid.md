

- StoreKit
- AppTransaction
-  bundleID 

Instance Property

# bundleID

The bundle identifier that the app transaction applies to.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let bundleID: String
```

## Discussion

The bundleID is the bundle identifier string that you entered in Xcode. For more information, see What is a bundle ID?

## See Also

### Getting app and version information

let appVersion: String

The app version that the app transaction applies to.

let originalAppVersion: String

The app version that the customer originally purchased from the App Store.

let appID: UInt64?

The unique identifier the App Store uses to identify the app.

let appVersionID: UInt64?

The number that the App Store uses to uniquely identify the version of the app.

