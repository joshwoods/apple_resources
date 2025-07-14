

- StoreKit
- SKProduct
-  downloadable Deprecated

Instance Property

# downloadable

A Boolean value that indicates whether the App Store has downloadable content for this product.

macOS 10.8–10.15Deprecated

``` source
var downloadable: Bool { get }
```

Deprecated

Use isDownloadable instead.

## Discussion

You can associate a set of data files with the App Store Connect record you created for a product. The value of this property is true if at least one file has been associated with the product.

## See Also

### Getting Downloadable Content Information

var isDownloadable: Bool

A Boolean value that indicates whether the App Store has downloadable content for this product.

Deprecated

var downloadContentLengths: [NSNumber]

The lengths of the downloadable files available for this product.

Deprecated

var downloadContentVersion: String

A string that identifies which version of the content is available for download.

Deprecated

