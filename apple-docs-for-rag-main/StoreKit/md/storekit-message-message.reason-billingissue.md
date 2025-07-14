

- StoreKit
- Message
- Message.Reason
-  billingIssue 

Type Property

# billingIssue

A message the App Store sends that informs people of a billing problem and enables them to update billing information.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+visionOS 1.0+

``` source
static let billingIssue: Message.Reason
```

## Mentioned in 

Testing failing subscription renewals and In-App Purchases

## Discussion

If an auto-renewable subscription fails to renew due to a billing issue, the subscription enters a billing retry state, and the App Store sends a message with the billingIssue reason.

When a billing issue is in effect, StoreKit displays a Billing Problem message sheet when your app launches, or when your app asks to display it.

The sheet informs people of the billing issue, and displays an in-app sheet to enable them to correct the issue without leaving your app. Note that people can also resolve billing issues outside of your app by navigating to the manage payments section in Apple ID settings. For more information, see support.apple.com.

Apple attempts to renew the subscription during the billing retry period, up to 60 days. During this period, the App Store sends the billingIssue message in the following intervals:

| Billing retry interval | Message frequency |
|------------------------|-------------------|
| Days 1–3               | Every 24 hours    |
| Days 4–16              | Every 72 hours    |
| Days 17–30             | Every 96 hours    |
| Days 31–60             | Every 120 hours   |

The App Store stops sending further messages when the user resolves the billing issue, cancels the subscription, or when the billing retry period ends. StoreKit ensures that the sheet appears only if the message is applicable when your app calls display(in:) or DisplayMessageAction.

For more information about the billing retry state, see isInBillingRetry in Product.SubscriptionInfo.RenewalInfo.

### Test the message in the sandbox environment

You can simulate billing issues in the sandbox environment to test how the system presents the billingIssue message in your app, and how your app handles it if you choose to delay or suppress its presentation. For more information, including step-by-step test cases, see Testing failing subscription renewals and In-App Purchases.

## See Also

### Getting the message reasons

static let generic: Message.Reason

A message the App Store sends for a generic reason.

static let priceIncreaseConsent: Message.Reason

A message the App Store sends when you increase the price of an auto-renewable subscription and the price increase requires the customer’s consent.

static let winBackOffer: Message.Reason

A message the App Store sends when the customer is eligible for a win-back offer that you configure in App Store Connect.

