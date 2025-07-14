

- App Store Server Notifications
-  transactionReason 

Type

# transactionReason

The cause of a purchase transaction, which indicates whether it’s a customer’s purchase or a renewal for an auto-renewable subscription that the system initiates.

App Store Server Notifications 2.8+

``` source
string transactionReason
```

## Possible Values 

`PURCHASE`  

The customer initiated the purchase, which may be for any in-app purchase type: consumable, non-consumable, non-renewing subscription, or auto-renewable subscription.

`RENEWAL`  

The App Store server initiated the purchase transaction to renew an auto-renewable subscription.

## Mentioned in 

App Store Server Notifications changelog

## Discussion

If a customer upgrades an auto-renewable subscription, the upgrade is effective immediately and the `transactionReason` is `PURCHASE`.

If a customer downgrades an auto-renewable subscription, the product change occurs on the subscription renewal date. The resulting `transactionReason` is `RENEWAL`.

