

- StoreKit
- Product
-  purchase(confirmIn:options:) 

Instance Method

# purchase(confirmIn:options:)

Processes a purchase for the product.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+tvOS 18.2+visionOS 2.2+

``` source
func purchase(
    confirmIn viewController: UIViewController,
    options: Set = []
) async throws -> Product.PurchaseResult
```

## Parameters 

`viewController`  

The view controller to show purchase confirmation UI in proximity to.

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

func purchase(confirmIn: NSWindow, options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Processes a purchase for the product.

struct PurchaseOption

Optional settings for a product purchase that add account information, purchase details, and offers, or that specify behaviors.

enum PurchaseResult

The result of a purchase.

enum PurchaseError

Error information for product purchase errors.

