

- StoreKit
- SKProduct
-  downloadContentLengths Deprecated

Instance Property

# downloadContentLengths

The lengths of the downloadable files available for this product.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.14–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var downloadContentLengths: [NSNumber] { get }
```

Deprecated

Hosted content is no longer supported

## Discussion

The array holds NSNumber objects, each of which holds a `long long` value that is the size of one of the downloadable files (in bytes).

## See Also

### Getting Downloadable Content Information

var isDownloadable: Bool

A Boolean value that indicates whether the App Store has downloadable content for this product.

Deprecated

var downloadContentVersion: String

A string that identifies which version of the content is available for download.

Deprecated

var downloadable: Bool

A Boolean value that indicates whether the App Store has downloadable content for this product.

Deprecated

