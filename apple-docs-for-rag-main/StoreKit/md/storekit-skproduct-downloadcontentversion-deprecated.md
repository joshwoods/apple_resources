

- StoreKit
- SKProduct
-  downloadContentVersion Deprecated

Instance Property

# downloadContentVersion

A string that identifies which version of the content is available for download.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.14–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var downloadContentVersion: String { get }
```

Deprecated

Hosted content is no longer supported

## Discussion

The version string is formatted as a series of integers separated by periods.

## See Also

### Getting Downloadable Content Information

var isDownloadable: Bool

A Boolean value that indicates whether the App Store has downloadable content for this product.

Deprecated

var downloadContentLengths: [NSNumber]

The lengths of the downloadable files available for this product.

Deprecated

var downloadable: Bool

A Boolean value that indicates whether the App Store has downloadable content for this product.

Deprecated

