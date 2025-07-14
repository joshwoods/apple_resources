

- App Store Server Notifications
-  expirationIntent 

Type

# expirationIntent

The reason a subscription expired.

App Store Server Notifications 2.0+

``` source
int32 expirationIntent
```

## Possible Values 

`1`  

The customer canceled their subscription.

`2`  

Billing error; for example, the customer’s payment information is no longer valid.

`3`  

The customer didn’t consent to an auto-renewable subscription price increase that requires customer consent, allowing the subscription to expire.

`4`  

The product wasn’t available for purchase at the time of renewal.

`5`  

The subscription expired for some other reason.

## See Also

### Subscripton renewal and expiration

type autoRenewStatus

The renewal status for an auto-renewable subscription.

type autoRenewProductId

The identifier of the product that renews at the next billing period.

type expiresDate

The UNIX time, in milliseconds, an auto-renewable subscription purchase expires or renews.

type isUpgraded

A Boolean value that indicates whether the customer upgraded to another subscription.

type renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

type renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

