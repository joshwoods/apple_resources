

- StoreKit
- Product
- Product.PurchaseOption
-  custom(key:value:) 

Type Method

# custom(key:value:)

Adds a number for a custom key to a purchase.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func custom(
    key: String,
    value: Double
) -> Product.PurchaseOption
```

## Parameters 

`key`  

The key for this custom option.

`value`  

The numerical value you assign to this custom option.

## Discussion

This custom purchase option doesn’t have any effect.

## See Also

### Setting custom purchase options

static func custom(key: String, value: Data) -> Product.PurchaseOption

Adds data for a custom key to a purchase.

static func custom(key: String, value: String) -> Product.PurchaseOption

Adds a string for a custom key to a purchase.

static func custom(key: String, value: Bool) -> Product.PurchaseOption

Adds a Boolean value for a custom key to a purchase.

