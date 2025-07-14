

- App Store Server Notifications
-  offerType 

Type

# offerType

The type of subscription offer.

App Store Server Notifications 2.0+

``` source
int32 offerType
```

## Possible Values 

`1`  

An introductory offer.

`2`  

A promotional offer.

`3`  

An offer with a subscription offer code.

`4`  

A win-back offer.

## Mentioned in 

App Store Server Notifications changelog

## Discussion

All offer types, except offer type `1`, have an offerIdentifier.

For more information about introductory offers, see Implementing introductory offers in your app. For more information about promotional offers, see Set up promotional offers for auto-renewable subscriptions. For more information about promo codes, see Promo codes overview.

## See Also

### Subscription offers

type eligibleWinBackOfferIds

An array of win-back offer identifiers that a customer is eligible to redeem, which sorts the identifiers to present the better offers first.

type offerIdentifier

The string identifier of a subscription offer that you create in App Store Connect.

type offerPeriod

The duration of the offer.

type offerDiscountType

The payment mode for a subscription offer for an auto-renewable subscription.

