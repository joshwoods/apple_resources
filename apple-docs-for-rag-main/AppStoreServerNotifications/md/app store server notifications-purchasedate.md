

- App Store Server Notifications
-  purchaseDate 

Type

# purchaseDate

The time that the App Store charged the customer’s account for a purchase, a restored product, a subscription, or a subscription renewal after a lapse.

App Store Server Notifications 2.0+

``` source
timestamp purchaseDate
```

## Discussion

The purchase date is in UNIX time, in milliseconds.

## See Also

### Purchase dates

type originalPurchaseDate

The purchase date of the transaction associated with the original transaction identifier.

type recentSubscriptionStartDate

The earliest start date of a subscription in a series of auto-renewable subscription purchases that ignores all lapses of paid service shorter than 60 days.

