

- StoreKit
- SKProductStorePromotionController
-  update(storePromotionVisibility:for:completionHandler:) Deprecated

Instance Method

# update(storePromotionVisibility:for:completionHandler:)

Updates the visibility of the product on the App Store, per device.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 11.0–18.0Deprecated

``` source
func update(
    storePromotionVisibility promotionVisibility: SKProductStorePromotionVisibility,
    for product: SKProduct,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func update(
    promotionVisibility: SKProductStorePromotionVisibility,
    for product: SKProduct
) async throws
```

Deprecated

Use Product.PromotionInfo.updateProductVisibility(\_:for:)

## Discussion

An in-app purchase product’s default visibility setting is set up in App Store Connect. You can override the default setting, or return it to the default set in App Store Connect using the values in SKProductStorePromotionVisibility.

Visibility settings apply per device.

## See Also

### Managing promoted product visibility

func fetchStorePromotionVisibility(for: SKProduct, completionHandler: ((SKProductStorePromotionVisibility, (any Error)?) -> Void)?)

Reads the visibility setting of a promoted product in the App Store for this device.

Deprecated

enum SKProductStorePromotionVisibility

The visibility settings that determine if an in-app purchase is visible on a device.

Deprecated

