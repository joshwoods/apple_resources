

- App Store Server API
-  originalPurchaseDate 

Type

# originalPurchaseDate

The purchase date of the transaction associated with the original transaction identifier.

App Store Server API 1.0+

``` source
timestamp originalPurchaseDate
```

## Discussion

The original purchase date is in UNIX time, in milliseconds.

## See Also

### Purchase dates

type purchaseDate

The time that the App Store charged the customer’s account for an In-App Purchase, a restored In-App Purchase, a subscription, or a subscription renewal after a lapse.

type recentSubscriptionStartDate

The earliest start date of a subscription in a series of auto-renewable subscription purchases that ignores all lapses of paid service shorter than 60 days.

