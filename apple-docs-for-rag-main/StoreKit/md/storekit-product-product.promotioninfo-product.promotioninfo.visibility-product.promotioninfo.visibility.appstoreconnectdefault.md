

- StoreKit
- Product
- Product.PromotionInfo
- Product.PromotionInfo.Visibility
-  Product.PromotionInfo.Visibility.appStoreConnectDefault 

Case

# Product.PromotionInfo.Visibility.appStoreConnectDefault

A visibility value for a promoted in-app purchase that uses the visibility setting from App Store Connect.

iOS 16.4+iPadOS 16.4+

``` source
case appStoreConnectDefault
```

## Mentioned in 

Supporting promoted In-App Purchases in your app

## Discussion

When a promoted in-app purchase has a visibility value of Product.PromotionInfo.Visibility.appStoreConnectDefault, the in-app purchase is:

- Visible if the setting in App Store Connect makes it visible

- Hidden if the setting in App Store Connect makes it hidden

Use this value to control the visibility for promoted in-app purchases in App Store Connect, globally, for all users. For example, if you have a product to promote on a holiday, start by manually setting it as hidden using App Store Connect. On the holiday, change the setting to make the promotion visible. If the promotion visibility in the app is the default (Product.PromotionInfo.Visibility.appStoreConnectDefault), it becomes visible for all users automatically.

For more information about the visibility settings in App Store Connect, see Promote in-app purchases.

## See Also

### Getting visibility states

case hidden

A visibility value that hides a promoted in-app purchase on the App Store on a user’s device.

case visible

A visibility value that makes a promoted in-app purchase visible on the App Store on a user’s device.

