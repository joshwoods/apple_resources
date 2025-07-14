

- StoreKit
- SKPaymentQueue
-  storefront Deprecated

Instance Property

# storefront

The App Store storefront of the device.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0DeprecatedtvOS 13.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var storefront: SKStorefront? { get }
```

Deprecated

Use Storefront.current

## Discussion

The storefront information tells you the device’s App Store region. You can use this information to display products that your app makes available in specific regions. You maintain your own list of product identifiers and the storefronts in which you make them available.

If the storefront changes during a transaction, StoreKit notifies your app by calling the paymentQueueDidChangeStorefront(_:) method of the SKPaymentTransactionObserver protocol. Implement paymentQueue(_:shouldContinue:in:) to indicate whether the transaction should continue with the new storefront.

Important

storefront is a synchronous API that may take significant time to return. Don’t use storefront in a time-sensitive thread, such as during app launch. To get asynchronous behavior, dispatch it to a separate queue, or use the asynchronous current property of Storefront instead.

