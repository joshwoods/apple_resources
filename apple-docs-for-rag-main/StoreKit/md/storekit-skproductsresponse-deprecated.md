

- StoreKit
-  SKProductsResponse Deprecated

Class

# SKProductsResponse

An App Store response to a request for information about a list of products.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKProductsResponse
```

Deprecated

Get products using Product.products(for:)

## Topics

### Response Information

var products: [SKProduct]

A list of products, one product for each valid product identifier provided in the original request.

var invalidProductIdentifiers: [String]

An array of product identifier strings that the App Store doesn’t recognize.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Product information

Loading in-app product identifiers

Load the unique identifiers for your in-app products to retrieve product information from the App Store.

Fetching product information from the App Store

Retrieve up-to-date information about the products for sale in your app to display to your customers.

class SKProductsRequest

An object that can retrieve localized information from the App Store about a specified list of products.

Deprecated

class SKProduct

Information about a registered product in App Store Connect.

Deprecated

