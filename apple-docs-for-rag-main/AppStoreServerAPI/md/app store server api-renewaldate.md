

- App Store Server API
-  renewalDate 

Type

# renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

App Store Server API 1.8+

``` source
timestamp renewalDate
```

## Mentioned in 

App Store Server API changelog

## Discussion

The `renewalDate` is a value that’s always present in the payload for auto-renewable subscriptions, even for expired subscriptions. This date indicates the expiration date of the most recent auto-renewable subscription purchase, including renewals, and may be in the past. For subscriptions that renew successfully, the renewalDate is the date when the subscription renews.

## See Also

### Subscription renewal and expiration

type autoRenewStatus

The renewal status for an auto-renewable subscription.

type autoRenewProductId

The identifier of the product that renews at the next billing period.

type expirationIntent

The reason an auto-renewable subscription expired.

type expiresDate

The UNIX time, in milliseconds, an auto-renewable subscription purchase expires or renews.

type isUpgraded

The Boolean value that indicates whether the customer upgraded to another subscription.

type renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

type status

The status of an auto-renewable subscription.

