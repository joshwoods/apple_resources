

- StoreKit
- Product
-  purchase(confirmIn:options:) 

Instance Method

# purchase(confirmIn:options:)

Initiates a purchase for the product with the App Store and displays the confirmation sheet.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func purchase(
    confirmIn scene: some UIScene,
    options: Set = []
) async throws -> Product.PurchaseResult
```

## Parameters 

`scene`  

The UIScene the system uses to show the purchase confirmation UI.

`options`  

A set of options (Product.PurchaseOption) you can associate with the purchase.

## Return Value

The result of the purchase, Product.PurchaseResult.

## Discussion

StoreKit provides several APIs you can use to enable customers to initiate a purchase. Before using purchase(confirmIn:options:), consider the following APIs and choose the one that best suits your app’s implementation:

- Use PurchaseAction for apps that use SwiftUI on any platform, including multi-scene apps for visionOS.

- Use purchase(confirmIn:options:) for apps that use UIKit.

- Use purchase(confirmIn:options:) for apps that run on macOS and use AppKit.

- Use purchase(options:) for apps that runs on watchOS.

Important

If you use StoreKit views such as ProductView, StoreView, or SubscriptionStoreView you don’t need to call any other API to initiate a purchase. StoreKit manages the purchase action automatically, including presenting the purchase confirmation UI. For more information, see StoreKit views.

This method may throw a Product.PurchaseError or StoreKitError.

## See Also

### Purchasing a product

func purchase(options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Initiates a purchase for the product with the App Store and displays the confirmation sheet.

func purchase(confirmIn: UIViewController, options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Processes a purchase for the product.

func purchase(confirmIn: NSWindow, options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Processes a purchase for the product.

struct PurchaseOption

Optional settings for a product purchase that add account information, purchase details, and offers, or that specify behaviors.

enum PurchaseResult

The result of a purchase.

enum PurchaseError

Error information for product purchase errors.

