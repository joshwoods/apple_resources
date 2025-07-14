

- StoreKit
- AdvancedCommerceProduct
-  AdvancedCommerceProduct.PurchaseOption 

Structure

# AdvancedCommerceProduct.PurchaseOption

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct PurchaseOption
```

## Topics

### Type Methods

static func onStorefrontChange(shouldContinuePurchase: (Storefront) -> Bool) -> AdvancedCommerceProduct.PurchaseOption

A closure that determines whether the transaction continues if the device’s App Store storefront changes during a transaction.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Initiating purchases

func purchase(compactJWS: String, confirmIn: NSWindow, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

func purchase(compactJWS: String, confirmIn: UIViewController, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

func purchase(compactJWS: String, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

typealias PurchaseResult

