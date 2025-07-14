

- StoreKit
- AppTransaction
-  shared 

Type Property

# shared

Gets the App Store-signed app transaction information for the app.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var shared: VerificationResult { get async throws }
```

## Discussion

Use this property to get a VerificationResult that contains the App Store-signed app transaction information for your app, including the first time the app launches. StoreKit automatically keeps the app transaction up-to-date.

This property throws an error if the AppTransaction isn’t available or if the user isn’t authenticated with the App Store. Getting an AppTransaction may require network connectivity.

The following example shows how to get the AppTransaction.

```
```

If your app fails to get an AppTransaction by accessing the shared property, see refresh().

