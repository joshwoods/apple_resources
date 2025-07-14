

- StoreKit
- AdvancedCommerceProduct
-  AdvancedCommerceProduct.PurchaseResult 

Type Alias

# AdvancedCommerceProduct.PurchaseResult

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
typealias PurchaseResult = Product.PurchaseResult
```

## See Also

### Initiating purchases

struct PurchaseOption

func purchase(compactJWS: String, confirmIn: NSWindow, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

func purchase(compactJWS: String, confirmIn: UIViewController, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

func purchase(compactJWS: String, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

