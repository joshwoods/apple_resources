

- StoreKit
- Product
- Product.PromotionInfo
-  visibility 

Instance Property

# visibility

A value that indicates whether the promoted in-app purchase is visible or hidden on the user’s device.

iOS 16.4+iPadOS 16.4+

``` source
var visibility: Product.PromotionInfo.Visibility
```

## Mentioned in 

Supporting promoted In-App Purchases in your app

## Discussion

To override the visibility of a promoted in-app purchase, set the visibility value and then call update() to save the change. You can also call updateProductVisibility(_:for:) to set the visibility.

The default value is Product.PromotionInfo.Visibility.appStoreConnectDefault.

## See Also

### Managing promotion visibility

enum Visibility

The visibility states for product promotion information.

static func updateProductVisibility(Product.PromotionInfo.Visibility, for: Product.ID) async throws

Updates a value that indicates whether a promoted in-app purchase appears in the App Store on the user’s device.

