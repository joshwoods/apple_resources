

- StoreKit
- SKPaymentTransactionObserver
-  paymentQueue(\_:shouldAddStorePayment:for:) Deprecated

Instance Method

# paymentQueue(\_:shouldAddStorePayment:for:)

Tells the observer when a user initiates an in-app purchase from the App Store.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 11.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
optional func paymentQueue(
    _ queue: SKPaymentQueue,
    shouldAddStorePayment payment: SKPayment,
    for product: SKProduct
) -> Bool
```

Deprecated

Use PurchaseIntent.intents

## Parameters 

`queue`  

The payment queue the app uses to make the payment request.

`payment`  

The payment request.

`product`  

The in-app purchase product.

## Return Value

Return `true` to continue the transaction in your app.

## Mentioned in 

Promoting In-App Purchases

Supporting promoted In-App Purchases in your app

## Discussion

Return `false` to defer or cancel the transaction.

If you return `false`, you can continue the transaction later by manually adding the SKPayment `payment` to the SKPaymentQueue `queue`.

## Discussion

The system calls this delegate method when the user starts an in-app purchase in the App Store, and the transaction continues in your app. Specifically, if your app is already installed, StoreKit calls this method automatically.

If your app isn’t installed when the user starts the in-app purchase in the App Store, the user receives a notification when the app installation is complete. StoreKit calls this method when the user taps the notification. Otherwise, if the user opens the app manually, StoreKit calls this method only if they open the app soon after they initiate the purchase.

Important

To enable promoted in-app purchases, your app needs to use either PurchaseIntent (starting in iOS 16.4) or paymentQueue(_:shouldAddStorePayment:for:) (starting in iOS 11). Don’t use both at the same time. If necessary, use conditional compilation to identify the OS version the app is running in. For more information, see Running code on a specific platform or OS version.

For more information, see Promoting In-App Purchases.

## See Also

### Handling promoted in-app purchases

Promoting In-App Purchases

Show promoted In-App Purchases on your product page and handle purchases that customers initiate on the App Store.

