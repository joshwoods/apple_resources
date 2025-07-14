

- StoreKit
- Message
- Message.Reason
-  winBackOffer 

Type Property

# winBackOffer

A message the App Store sends when the customer is eligible for a win-back offer that you configure in App Store Connect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
static let winBackOffer: Message.Reason
```

## Mentioned in 

Merchandising win-back offers in your app

Supporting win-back offers in your app

Testing win-back offers in the sandbox environment

## Discussion

If the customer is eligible for a win-back offer, StoreKit displays the win-back offer message when the app launches. If your app customizes the way it displays win-back offers, you can suppress this message, as described in Message.

For more information, see Merchandising win-back offers in your app.

## See Also

### Getting the message reasons

static let billingIssue: Message.Reason

A message the App Store sends that informs people of a billing problem and enables them to update billing information.

static let generic: Message.Reason

A message the App Store sends for a generic reason.

static let priceIncreaseConsent: Message.Reason

A message the App Store sends when you increase the price of an auto-renewable subscription and the price increase requires the customer’s consent.

