

- App Store Server Notifications
-  renewalPrice 

Type

# renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

App Store Server Notifications 2.12+

``` source
int64 renewalPrice
```

## Discussion

This value represents the renewal price, in milliunits of the currency, of the auto-renewable subscription. One unit of the currency equals 1000 milliunits.

If the next billing period includes an offer specified by the offerIdentifier, the renewalPrice value reflects the discount.

Important

For financial and accounting purposes, use the App Store Connect reporting tools. For more information, see Download financial reports and Overview of reporting tools.

To determine the storefront, use the storefront value in the transaction. Don’t use the currency value to infer the storefront.

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

type renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

