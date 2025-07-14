

- StoreKit
- SKProductStorePromotionController
-  update(storePromotionOrder:completionHandler:) Deprecated

Instance Method

# update(storePromotionOrder:completionHandler:)

Overrides the promoted product order on this device.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 11.0–18.0Deprecated

``` source
func update(
    storePromotionOrder promotionOrder: [SKProduct],
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func update(promotionOrder: [SKProduct]) async throws
```

Deprecated

Use Product.PromotionInfo.updateProductOrder(byID:)

## Mentioned in 

Promoting In-App Purchases

## Discussion

The default order of promoted in-app purchase products is set in App Store Connect. You can override this order per device. For example, you can promote an in-app purchase product that unlocks a specific level in your game when a user reaches the level immediately before the specified level.

To override the default product order, put the product information for the subset of products you want to reorder into an array, in the order you want them to appear in. Pass the array to the update(storePromotionOrder:completionHandler:) method. The products in the array are shown at the beginning of the list, followed by the remaining in-app purchase products, which are listed in the same relative order that you set in App Store Connect.

To cancel order overrides, send an empty product array to the update(storePromotionOrder:completionHandler:) method. The in-app purchase products will be displayed in the default order.

## See Also

### Managing promoted product order

func fetchStorePromotionOrder(completionHandler: (([SKProduct], (any Error)?) -> Void)?)

Reads the product order override that determines the promoted product order on this device.

Deprecated

