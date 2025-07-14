

- StoreKit
- SKProductStorePromotionController
-  fetchStorePromotionVisibility(for:completionHandler:) Deprecated

Instance Method

# fetchStorePromotionVisibility(for:completionHandler:)

Reads the visibility setting of a promoted product in the App Store for this device.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 11.0–18.0Deprecated

``` source
func fetchStorePromotionVisibility(
    for product: SKProduct,
    completionHandler: ((SKProductStorePromotionVisibility, (any Error)?) -> Void)? = nil
)
```

``` source
func promotionVisibility(for product: SKProduct) async throws -> SKProductStorePromotionVisibility
```

Deprecated

Get visibility from Product.PromotionInfo.currentOrder

## Mentioned in 

Promoting In-App Purchases

## Discussion

The default visibility for a promoted product is set in App Store Connect. Call fetchStorePromotionVisibility(for:completionHandler:) to determine if a product’s visibility is set to the default value or if it has been overridden to be hidden or shown.

## See Also

### Managing promoted product visibility

func update(storePromotionVisibility: SKProductStorePromotionVisibility, for: SKProduct, completionHandler: (((any Error)?) -> Void)?)

Updates the visibility of the product on the App Store, per device.

Deprecated

enum SKProductStorePromotionVisibility

The visibility settings that determine if an in-app purchase is visible on a device.

Deprecated

