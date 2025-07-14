

- StoreKit
- SKPaymentQueueDelegate
-  paymentQueue(\_:shouldContinue:in:) Deprecated

Instance Method

# paymentQueue(\_:shouldContinue:in:)

Asks the delegate whether to continue the transaction if the device’s App Store storefront changes during a transaction.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0DeprecatedtvOS 13.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
optional func paymentQueue(
    _ paymentQueue: SKPaymentQueue,
    shouldContinue transaction: SKPaymentTransaction,
    in newStorefront: SKStorefront
) -> Bool
```

Deprecated

Pass Product.PurchaseOption.onStorefrontChange(shouldContinuePurchase:) to product.purchase(options:)

## Discussion

StoreKit calls this delegate method if the storefront changes while processing a transaction.

- Return `true` if you wish to continue the transaction within the updated storefront.

- Return `false` to stop the transaction. The transaction will fail with the error SKError.Code.storeProductNotAvailable. In this case, consider displaying a message to the user indicating that the product isn’t available in the current storefront.

If the delegate isn’t implemented, paymentQueue(_:shouldContinue:in:) defaults to `true`.

This call times out after approximately one second, defaulting to `false` and causing the transaction to fail. The delegate should return as quickly as possible. Don’t perform any networking calls in this method. Your app should cache product availability information locally before starting a transaction.

See SKStorefront for more information.

