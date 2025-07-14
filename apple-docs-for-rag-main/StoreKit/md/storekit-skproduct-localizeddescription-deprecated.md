

- StoreKit
- SKProduct
-  localizedDescription Deprecated

Instance Property

# localizedDescription

A description of the product.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var localizedDescription: String { get }
```

Deprecated

Use Product.description

## Discussion

The description’s language is determined by the storefront that the user’s device is connected to, not the preferred language set on the device.

## See Also

### Related Documentation

class SKStorefront

An object containing the location and unique identifier of an Apple App Store storefront.

Deprecated

### Getting Product Attributes

var localizedTitle: String

The name of the product.

Deprecated

var contentVersion: String

A string that identifies the version of the content.

Deprecated

var isFamilyShareable: Bool

A Boolean value that indicates whether the product is available for Family Sharing in App Store Connect.

Deprecated

var contentLengths: [NSNumber]

The total size of the content, in bytes.

Deprecated

