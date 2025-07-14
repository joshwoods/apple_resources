

- App Store Server API
-  offerIdentifier 

Type

# offerIdentifier

The string identifier of a subscription offer that you create in App Store Connect.

App Store Server API 1.0+

``` source
string offerIdentifier
```

## Discussion

The `offerIdentifier` is a string that you provide in App Store Connect when you set up a subscription offer. All offer types (offerType) have offer identifiers, except for introductory offers.

For more information about subscription offers, see Providing subscription offers. For information about configuring the various types of subscription offers in App Store Connect, see:

- Set up offer codes

- Set up introductory offers for auto-renewable subscriptions

- Set up promotional offers for auto-renewable subscriptions

- Set up win-back offers

## See Also

### Subscription offers

type eligibleWinBackOfferIds

An array of win-back offer identifiers that a customer is eligible to redeem, which sorts the identifiers with the best offers first.

type offerPeriod

The duration of the offer.

type offerType

The type of subscription offer.

type offerDiscountType

The payment mode for subscription offers on an auto-renewable subscription.

