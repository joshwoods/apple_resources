

- App Store Server Notifications
-  isUpgraded 

Type

# isUpgraded

A Boolean value that indicates whether the customer upgraded to another subscription.

App Store Server Notifications 2.0+

``` source
boolean isUpgraded
```

## Discussion

If `isUpgraded` is `true`, the customer has upgraded the subscription represented by this transaction to another subscription. This value appears in the transaction only when the value is `true`. To determine the service that the customer is entitled to, look for another transaction that has a subscription with a higher level of service. For more information about subscription groups and levels of service, see Auto-renewable Subscriptions.

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

type renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

type renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

