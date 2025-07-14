

- StoreKit
- SKProduct
-  isDownloadable Deprecated

Instance Property

# isDownloadable

A Boolean value that indicates whether the App Store has downloadable content for this product.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.15–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var isDownloadable: Bool { get }
```

Deprecated

Hosted content is no longer supported

## Discussion

You can associate a set of data files with the App Store Connect record you created for a product. The value of this property is true if at least one file has been associated with the product.

## See Also

### Getting Downloadable Content Information

var downloadContentLengths: [NSNumber]

The lengths of the downloadable files available for this product.

Deprecated

var downloadContentVersion: String

A string that identifies which version of the content is available for download.

Deprecated

var downloadable: Bool

A Boolean value that indicates whether the App Store has downloadable content for this product.

Deprecated

