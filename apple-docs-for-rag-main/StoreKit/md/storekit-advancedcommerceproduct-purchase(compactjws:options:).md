

- StoreKit
- AdvancedCommerceProduct
-  purchase(compactJWS:options:) 

Instance Method

# purchase(compactJWS:options:)

Processes a purchase for the product.

watchOS 11.4+

``` source
@MainActor
func purchase(
    compactJWS: String,
    options: Set = []
) async throws -> AdvancedCommerceProduct.PurchaseResult
```

## Parameters 

`compactJWS`  

The compact JSON Web Signature (JWS) string for the operation.

`options`  

A set of purchase options.

## Return Value

The result of the purchase.

## Discussion

Throws

A `PurchaseError`, `StoreKitError`, or `InvalidRequest` error.

## See Also

### Initiating purchases

struct PurchaseOption

func purchase(compactJWS: String, confirmIn: NSWindow, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

func purchase(compactJWS: String, confirmIn: UIViewController, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

typealias PurchaseResult

