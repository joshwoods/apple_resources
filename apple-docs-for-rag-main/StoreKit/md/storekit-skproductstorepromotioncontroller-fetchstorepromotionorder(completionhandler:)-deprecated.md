

- StoreKit
- SKProductStorePromotionController
-  fetchStorePromotionOrder(completionHandler:) Deprecated

Instance Method

# fetchStorePromotionOrder(completionHandler:)

Reads the product order override that determines the promoted product order on this device.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 11.0–18.0Deprecated

``` source
func fetchStorePromotionOrder(completionHandler: (([SKProduct], (any Error)?) -> Void)? = nil)
```

``` source
func promotionOrder() async throws -> [SKProduct]
```

Deprecated

Use Product.PromotionInfo.currentOrder

## Mentioned in 

Promoting In-App Purchases

## Discussion

This function returns an array of promoted products whose order is overridden on the given device.

If all the products appear in the default order, this method returns an empty array.

## See Also

### Managing promoted product order

func update(storePromotionOrder: [SKProduct], completionHandler: (((any Error)?) -> Void)?)

Overrides the promoted product order on this device.

Deprecated

