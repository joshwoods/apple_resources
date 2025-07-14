

- StoreKit
- Product
- Product.PromotionInfo
-  updateAll(\_:) 

Type Method

# updateAll(\_:)

Sets the order and visibility of all the promoted products and saves your changes.

iOS 16.4+iPadOS 16.4+

``` source
static func updateAll(_ promotions: some Collection) async throws
```

## Parameters 

`promotions`  

A collection of Product.PromotionInfo objects that you list in the order they are to appear in the App Store on the user’s device. Use an empty collection to cancel previous changes.

## Mentioned in 

Supporting promoted In-App Purchases in your app

## Discussion

Call this static method to set the order of promoted in-app purchases for the user. Calling this method overrides any previous order and visibility that you set for this user.

To remove a promoted in-app purchase so it doesn’t display for a user, there are two options:

- Don’t include it in the `promotions` collection.

- Change its visibility value to Product.PromotionInfo.Visibility.hidden.

To set the order of promoted in-app purchases using product identifiers instead of Product.PromotionInfo objects, see updateProductOrder(byID:).

### Cancel overrides

To cancel the order and visibility changes you make, send an empty collection in `promotions`. All in-app purchases then display in the default order.

## See Also

### Updating order and visibility

func update() async throws

Saves your changes to the promoted product’s visibility.

