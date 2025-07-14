

- App Store Server API
-  status 

Type

# status

The status of an auto-renewable subscription.

App Store Server API 1.0+

``` source
int32 status
```

## Possible Values 

`1`  

The auto-renewable subscription is active.

`2`  

The auto-renewable subscription is expired.

`3`  

The auto-renewable subscription is in a billing retry period.

`4`  

The auto-renewable subscription is in a Billing Grace Period.

`5`  

The auto-renewable subscription is revoked. The App Store refunded the transaction or revoked it from Family Sharing.

## Discussion

For more information about the Billing Grace Period, see Enable Billing Grace Period for auto-renewable subscriptions.

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

type renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

type renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

