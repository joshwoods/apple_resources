

- StoreKit
- Message
- Message.Reason
-  priceIncreaseConsent 

Type Property

# priceIncreaseConsent

A message the App Store sends when you increase the price of an auto-renewable subscription and the price increase requires the customer’s consent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
static let priceIncreaseConsent: Message.Reason
```

## Discussion

For more information about managing prices, see Managing Prices and Manage pricing for auto-renewable subscriptions.

## See Also

### Getting the message reasons

static let billingIssue: Message.Reason

A message the App Store sends that informs people of a billing problem and enables them to update billing information.

static let generic: Message.Reason

A message the App Store sends for a generic reason.

static let winBackOffer: Message.Reason

A message the App Store sends when the customer is eligible for a win-back offer that you configure in App Store Connect.

