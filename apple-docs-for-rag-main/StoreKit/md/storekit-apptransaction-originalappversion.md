

- StoreKit
- AppTransaction
-  originalAppVersion 

Instance Property

# originalAppVersion

The app version that the customer originally purchased from the App Store.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let originalAppVersion: String
```

## Mentioned in 

Supporting business model changes by using the app transaction

## Discussion

Use this value to determine which app version the customer first purchased or downloaded. This value is comparable to the appVersion value.

The originalAppVersion remains constant and doesn’t change when the customer upgrades the app. The string value contains the original value of the CFBundleShortVersionString for apps running in macOS, and the original value of the CFBundleVersion for apps running on all other platforms.

In the sandbox testing environment, the originalAppVersion value is always `1.0`.

For more information about using the originalAppVersion, see Supporting business model changes by using the app transaction.

## See Also

### Getting app and version information

let bundleID: String

The bundle identifier that the app transaction applies to.

let appVersion: String

The app version that the app transaction applies to.

let appID: UInt64?

The unique identifier the App Store uses to identify the app.

let appVersionID: UInt64?

The number that the App Store uses to uniquely identify the version of the app.

