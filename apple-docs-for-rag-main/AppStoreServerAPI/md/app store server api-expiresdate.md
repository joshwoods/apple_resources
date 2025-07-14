

- App Store Server API
-  expiresDate 

Type

# expiresDate

The UNIX time, in milliseconds, an auto-renewable subscription purchase expires or renews.

App Store Server API 1.0+

``` source
timestamp expiresDate
```

## Discussion

The `expiresDate` is a static value that applies for each transaction. When the auto-renewable subscription renews, the App Store creates a new transaction with a new expiresDate.

## See Also

### Subscription renewal and expiration

type autoRenewStatus

The renewal status for an auto-renewable subscription.

type autoRenewProductId

The identifier of the product that renews at the next billing period.

type expirationIntent

The reason an auto-renewable subscription expired.

type isUpgraded

The Boolean value that indicates whether the customer upgraded to another subscription.

type renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

type renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

type status

The status of an auto-renewable subscription.

