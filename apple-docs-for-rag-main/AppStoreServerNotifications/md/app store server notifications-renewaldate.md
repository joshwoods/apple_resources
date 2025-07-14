

- App Store Server Notifications
-  renewalDate 

Type

# renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

App Store Server Notifications 2.8+

``` source
timestamp renewalDate
```

## Discussion

The `renewalDate` is a value that’s always present in the payload for auto-renewable subscriptions, even for expired subscriptions. This date indicates the expiration date of the most recent auto-renewable subscription purchase, including renewals, and may be in the past. For subscriptions that renew successfully, the `renewalDate` is the date when the subscription renews.

## See Also

### Subscripton renewal and expiration

type autoRenewStatus

The renewal status for an auto-renewable subscription.

type autoRenewProductId

The identifier of the product that renews at the next billing period.

type expirationIntent

The reason a subscription expired.

type expiresDate

The UNIX time, in milliseconds, an auto-renewable subscription purchase expires or renews.

type isUpgraded

A Boolean value that indicates whether the customer upgraded to another subscription.

type renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

