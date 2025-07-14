

- StoreKit
- AdvancedCommerceProduct
-  purchase(compactJWS:confirmIn:options:) 

Instance Method

# purchase(compactJWS:confirmIn:options:)

Processes a purchase for the product.

iOS 18.4+iPadOS 18.4+tvOS 18.4+visionOS 2.4+

``` source
func purchase(
    compactJWS: String,
    confirmIn viewController: UIViewController,
    options: Set = []
) async throws -> AdvancedCommerceProduct.PurchaseResult
```

## Parameters 

`compactJWS`  

The compact JSON Web Signature (JWS) string for the operation.

`viewController`  

The window the system uses to display purchase confirmation UI in proximity to.

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

func purchase(compactJWS: String, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

typealias PurchaseResult

