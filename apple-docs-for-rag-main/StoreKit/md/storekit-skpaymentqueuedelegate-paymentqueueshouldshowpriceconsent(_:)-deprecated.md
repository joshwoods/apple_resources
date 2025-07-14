

- StoreKit
- SKPaymentQueueDelegate
-  paymentQueueShouldShowPriceConsent(\_:) Deprecated

Instance Method

# paymentQueueShouldShowPriceConsent(\_:)

Asks the delegate whether to immediately display a price consent sheet.

iOS 13.4–18.0DeprecatediPadOS 13.4–18.0DeprecatedMac Catalyst 13.4–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
optional func paymentQueueShouldShowPriceConsent(_ paymentQueue: SKPaymentQueue) -> Bool
```

Deprecated

Use Message.messages and Message.display(in:)

## Mentioned in 

Handling Subscriptions Billing

## Discussion

This method applies only to auto-renewable subscription price increases that require customer consent.

The default return value for this optional method is `true`. By default, the system displays the price consent sheet when you increase the subscription price in App Store Connect and the subscriber hasn’t yet taken action.

The system calls your delegate’s method, if appropriate, when you add the first observer to SKPaymentQueue, and any time the app comes to foreground.

If you return `false`, the system won’t show the price consent sheet. You can choose to display it later by calling showPriceConsentIfNeeded(). You may want to delay showing the sheet if it would interrupt your user’s interaction in your app.

Note

When you increase the price of an auto-renewable subscription and it requires customer consent, Apple informs affected subscribers through an email, push notification, and an in-app price consent sheet and asks them to agree to the new price. If they don’t agree or take no action, their subscription expires at the end of their current billing cycle. For more information, see Managing Prices and Manage pricing for auto-renewable subscriptions.

In Mac apps built with Mac Catalyst, the system doesn’t show the price consent sheet regardless of the return value.

## See Also

### Related Documentation

func showPriceConsentIfNeeded()

Asks the system to display the price consent sheet if the user hasn’t yet responded to a subscription price increase.

Deprecated

