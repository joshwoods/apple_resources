

- StoreKit
- Product
- Product.PromotionInfo
-  update() 

Instance Method

# update()

Saves your changes to the promoted product’s visibility.

iOS 16.4+iPadOS 16.4+

``` source
func update() async throws
```

## Mentioned in 

Supporting promoted In-App Purchases in your app

## Discussion

If you change the visibility value by setting it directly, call update() to save your changes to the App Store server. Changes take effect after you call update() or updateAll(_:).

## See Also

### Updating order and visibility

static func updateAll(some Collection&lt;Product.PromotionInfo>) async throws

Sets the order and visibility of all the promoted products and saves your changes.

