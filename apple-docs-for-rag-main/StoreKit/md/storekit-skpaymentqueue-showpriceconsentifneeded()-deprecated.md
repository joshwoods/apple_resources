

- StoreKit
- SKPaymentQueue
-  showPriceConsentIfNeeded() Deprecated

Instance Method

# showPriceConsentIfNeeded()

Asks the system to display the price consent sheet if the user hasn’t yet responded to a subscription price increase.

iOS 13.4–18.0DeprecatediPadOS 13.4–18.0DeprecatedMac Catalyst 13.4–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func showPriceConsentIfNeeded()
```

Deprecated

Use Message.messages and Message.display(in:)

## Mentioned in 

Handling Subscriptions Billing

## Discussion

Call this method if the system called your delegate’s paymentQueueShouldShowPriceConsent(_:) method, and you chose to delay showing the price consent sheet.

This function displays the price consent sheet if both of the following are true:

- You’ve increased the price of the subscription in App Store Connect.

- The subscriber hasn’t yet responded to a price consent query.

Otherwise, this function has no effect.

Note

When you increase the price of a subscription, Apple informs affected subscribers through an email, push notification, and in-app price consent sheet and asks them to agree to the new price. If they don’t agree or take no action, their subscription expires at the end of their current billing cycle. For more information, see Managing Prices and Manage pricing for auto-renewable subscriptions.

In Mac apps built with Mac Catalyst, this function has no effect.

## See Also

### Related Documentation

func paymentQueueShouldShowPriceConsent(SKPaymentQueue) -> Bool

Asks the delegate whether to immediately display a price consent sheet.

Deprecated

