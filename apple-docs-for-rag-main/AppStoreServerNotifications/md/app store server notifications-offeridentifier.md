

- App Store Server Notifications
-  offerIdentifier 

Type

# offerIdentifier

The string identifier of a subscription offer that you create in App Store Connect.

App Store Server Notifications 2.0+

``` source
string offerIdentifier
```

## Discussion

The `offerIdentifier` is a string that you provide in App Store Connect when you set up a subscription offer. All offer types (offerType) have offer identifiers, except for introductory offers.

For more information on offer codes, see Supporting subscription offer codes in your app and Set up offer codes. For more information on promotional offers, see Set up promotional offers for auto-renewable subscriptions.

## See Also

### Subscription offers

type eligibleWinBackOfferIds

An array of win-back offer identifiers that a customer is eligible to redeem, which sorts the identifiers to present the better offers first.

type offerPeriod

The duration of the offer.

type offerType

The type of subscription offer.

type offerDiscountType

The payment mode for a subscription offer for an auto-renewable subscription.

