

- StoreKit
- Product
-  purchase(confirmIn:options:) 

Instance Method

# purchase(confirmIn:options:)

Processes a purchase for the product.

macOS 15.2+

``` source
func purchase(
    confirmIn window: NSWindow,
    options: Set = []
) async throws -> Product.PurchaseResult
```

## Parameters 

`window`  

The window to show purchase confirmation UI in proximity to.

`options`  

A set of options to configure the purchase.

## Return Value

The result of the purchase

## Discussion

Throws

A `PurchaseError` or `StoreKitError`.

## See Also

### Purchasing a product

func purchase(options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Initiates a purchase for the product with the App Store and displays the confirmation sheet.

func purchase(confirmIn: some UIScene, options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Initiates a purchase for the product with the App Store and displays the confirmation sheet.

func purchase(confirmIn: UIViewController, options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Processes a purchase for the product.

struct PurchaseOption

Optional settings for a product purchase that add account information, purchase details, and offers, or that specify behaviors.

enum PurchaseResult

The result of a purchase.

enum PurchaseError

Error information for product purchase errors.

