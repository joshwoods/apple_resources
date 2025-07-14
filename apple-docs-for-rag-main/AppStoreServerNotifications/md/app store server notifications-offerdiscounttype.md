

- App Store Server Notifications
-  offerDiscountType 

Type

# offerDiscountType

The payment mode for a subscription offer for an auto-renewable subscription.

App Store Server Notifications 2.9+

``` source
string offerDiscountType
```

## Possible Values 

`FREE_TRIAL`  

A payment mode of a product discount that indicates a free trial.

`PAY_AS_YOU_GO`  

A payment mode of a product discount that customers pay over a single or multiple billing periods.

`PAY_UP_FRONT`  

A payment mode of a product discount that customers pay up front.

## Mentioned in 

App Store Server Notifications changelog

## Discussion

You set up subscription offers and determine the payment mode when you configure subscriptions in App Store Connect. For more information about the Free Trial, Pay As You Go, and Pay Up Front payment modes, see Pricing and availability.

For more information about configuring subscription offers, see: Set up introductory offers for auto-renewable subscriptions, Set up promotional offers for auto-renewable subscriptions, and Set up offer codes.

## See Also

### Subscription offers

type eligibleWinBackOfferIds

An array of win-back offer identifiers that a customer is eligible to redeem, which sorts the identifiers to present the better offers first.

type offerIdentifier

The string identifier of a subscription offer that you create in App Store Connect.

type offerPeriod

The duration of the offer.

type offerType

The type of subscription offer.

