

- StoreKit
- PurchaseIntent
-  offer 

Instance Property

# offer

The subscription offer that the customer redeems outside of your app.

iOS 18.0+iPadOS 18.0+Mac Catalyst 16.4+macOS 15.0+

``` source
let offer: Product.SubscriptionOffer?
```

## Mentioned in 

Supporting win-back offers in your app

## Discussion

The system populates this value if the customer redeems a winBack offer type outside of your app. Add this offer to the purchase options. For more information and a code example, see the Handle win-back offers redeemed outside of your app section of Supporting win-back offers in your app.

