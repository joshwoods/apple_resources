

- StoreKit
- Storefront
-  current 

Type Property

# current

The current App Store storefront for product purchases.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var current: Storefront? { get async }
```

## Discussion

Use current to determine a customer’s current storefront region and offer in-app products suitable for that region. You maintain your own list of product identifiers and the storefronts in which you make them available.

## See Also

### Storefront information

struct Storefront

The region and unique identifier of the App Store storefront for the device.

static var updates: Storefront.Storefronts

The asynchronous sequence that emits storefront information when the system updates the storefront.

