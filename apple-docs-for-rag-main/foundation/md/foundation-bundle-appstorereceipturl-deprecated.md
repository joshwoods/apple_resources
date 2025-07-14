

- Foundation
- Bundle
-  appStoreReceiptURL Deprecated

Instance Property

# appStoreReceiptURL

The file URL for the bundle’s App Store receipt.

iOS 7.0–18.0DeprecatediPadOS 7.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 2.0–11.0Deprecated

``` source
var appStoreReceiptURL: URL? { get }
```

Deprecated

Use AppTransaction.shared and Transaction.all from StoreKit.framework instead

## Discussion

Note

The receipt isn’t necessary if you use AppTransaction to validate the app download, or Transaction to validate in-app purchases. Only use the receipt if your app uses the Original API for In-App Purchase, or needs the receipt to validate the app download because it can’t use AppTransaction.

Use this app bundle property to locate the app receipt if it’s present; this property is `nil` if the receipt isn’t present. In the rare case a receipt is invalid or missing in an app that a user downloads from the App Store, use SKReceiptRefreshRequest to request a new receipt. For information about validating receipts, see Choosing a receipt validation technique.

You can’t use the general best practice of weak linking using the responds(to:) method here; the method’s implementation uses the doesNotRecognizeSelector(_:) method.

### Get the receipt in testing environments

Receipts aren’t initially present in iOS and iPadOS apps in the sandbox environment and in Xcode. Apps get a receipt after the tester completes the first in-app purchase. When your app checks appStoreReceiptURL and finds that it’s `nil`, assume the tester is a new customer and has no access to premium content. For Mac apps running in TestFlight, the receipt is always present.

## See Also

### Getting the Standard Bundle Directories

var resourceURL: URL?

The file URL of the bundle’s subdirectory containing resource files.

var executableURL: URL?

The file URL of the receiver’s executable file.

var privateFrameworksURL: URL?

The file URL of the bundle’s subdirectory containing private frameworks.

var sharedFrameworksURL: URL?

The file URL of the receiver’s subdirectory containing shared frameworks.

var builtInPlugInsURL: URL?

The file URL of the receiver’s subdirectory containing plug-ins.

func url(forAuxiliaryExecutable: String) -> URL?

Returns the file URL of the executable with the specified name in the receiver’s bundle.

var sharedSupportURL: URL?

The file URL of the bundle’s subdirectory containing shared support files.

var resourcePath: String?

The full pathname of the bundle’s subdirectory containing resources.

var executablePath: String?

The full pathname of the receiver’s executable file.

var privateFrameworksPath: String?

The full pathname of the bundle’s subdirectory containing private frameworks.

var sharedFrameworksPath: String?

The full pathname of the bundle’s subdirectory containing shared frameworks.

var builtInPlugInsPath: String?

The full pathname of the receiver’s subdirectory containing plug-ins.

func path(forAuxiliaryExecutable: String) -> String?

Returns the full pathname of the executable with the specified name in the receiver’s bundle.

var sharedSupportPath: String?

The full pathname of the bundle’s subdirectory containing shared support files.

