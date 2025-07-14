

- StoreKit
- Product
-  Product.ProductType 

Structure

# Product.ProductType

The types of in-app purchases.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ProductType
```

## Topics

### Getting the Product Type

static let consumable: Product.ProductType

A consumable in-app purchase.

static let nonConsumable: Product.ProductType

A non-consumable in-app purchase.

static let nonRenewable: Product.ProductType

A non-renewing subscription.

static let autoRenewable: Product.ProductType

An auto-renewable subscription.

### Getting a Localized Description

var localizedDescription: String

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting product identifiers and type

let id: String

The unique product identifier.

let type: Product.ProductType

The in-app purchase product type.

