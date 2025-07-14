

- App Store Server API
-  offerDiscountType 

Type

# offerDiscountType

The payment mode for subscription offers on an auto-renewable subscription.

App Store Server API 1.10+

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

App Store Server API changelog

## Discussion

You set up subscription offers and determine the payment mode when you configure subscriptions in App Store Connect. For more information about the free trial, pay as you go, and pay up front payment modes, see Pricing and availability.

For more information on subscription offers, see Providing subscription offers.

## See Also

### Subscription offers

type eligibleWinBackOfferIds

An array of win-back offer identifiers that a customer is eligible to redeem, which sorts the identifiers with the best offers first.

type offerIdentifier

The string identifier of a subscription offer that you create in App Store Connect.

type offerPeriod

The duration of the offer.

type offerType

The type of subscription offer.

