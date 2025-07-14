

- App Store Server API
-  offerPeriod 

Type

# offerPeriod

The duration of the offer.

App Store Server API 1.15+

``` source
string offerPeriod
```

## Mentioned in 

App Store Server API changelog

## Discussion

This field is in ISO 8601 duration format.

The following table shows examples of offer period values.

| Single period length | Period count | Offer period value |
|----------------------|--------------|--------------------|
| 1 month              | 1            | `P1M`              |
| 1 month              | 2            | `P2M`              |
| 3 days               | 1            | `P3D`              |

## See Also

### Subscription offers

type eligibleWinBackOfferIds

An array of win-back offer identifiers that a customer is eligible to redeem, which sorts the identifiers with the best offers first.

type offerIdentifier

The string identifier of a subscription offer that you create in App Store Connect.

type offerType

The type of subscription offer.

type offerDiscountType

The payment mode for subscription offers on an auto-renewable subscription.

