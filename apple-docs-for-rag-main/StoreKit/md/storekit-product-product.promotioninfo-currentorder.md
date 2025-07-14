

- StoreKit
- Product
- Product.PromotionInfo
-  currentOrder 

Type Property

# currentOrder

Gets the customized order of the promotion info objects the represent promoted products.

iOS 16.4+iPadOS 16.4+

``` source
static var currentOrder: [Product.PromotionInfo] { get async throws }
```

## Mentioned in 

Supporting promoted In-App Purchases in your app

## Discussion

This asynchronous array returns a list of Product.PromotionInfo objects in the custom order they appear in on the device.

Note

This list is empty if you don’t override the order, and the App Store displays the products in their default order.

For information about setting the default order using App Store Connect, see Promote in-app purchases.

