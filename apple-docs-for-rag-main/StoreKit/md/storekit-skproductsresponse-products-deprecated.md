

- StoreKit
- SKProductsResponse
-  products Deprecated

Instance Property

# products

A list of products, one product for each valid product identifier provided in the original request.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var products: [SKProduct] { get }
```

Deprecated

Get products using Product.products(for:)

## Discussion

The array consists of a list of SKProduct objects.

## See Also

### Related Documentation

In-App Purchase Programming Guide

### Response Information

var invalidProductIdentifiers: [String]

An array of product identifier strings that the App Store doesn’t recognize.

Deprecated

