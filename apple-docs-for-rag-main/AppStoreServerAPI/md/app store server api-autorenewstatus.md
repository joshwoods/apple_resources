

- App Store Server API
-  autoRenewStatus 

Type

# autoRenewStatus

The renewal status for an auto-renewable subscription.

App Store Server API 1.0+

``` source
int32 autoRenewStatus
```

## Possible Values 

`0`  

Automatic renewal is off. The customer has turned off automatic renewal for the subscription, and it won’t renew at the end of the current subscription period.

`1`  

Automatic renewal is on. The subscription renews at the end of the current subscription period.

## See Also

### Subscription renewal and expiration

type autoRenewProductId

The identifier of the product that renews at the next billing period.

type expirationIntent

The reason an auto-renewable subscription expired.

type expiresDate

The UNIX time, in milliseconds, an auto-renewable subscription purchase expires or renews.

type isUpgraded

The Boolean value that indicates whether the customer upgraded to another subscription.

type renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

type renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

type status

The status of an auto-renewable subscription.

