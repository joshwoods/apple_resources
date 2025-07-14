

- App Store Server Notifications
-  revocationReason 

Type

# revocationReason

The reason for a refunded transaction.

App Store Server Notifications 2.0+

``` source
int32 revocationReason
```

## Possible Values 

`0`  

The App Store refunded the transaction on behalf of the customer for other reasons, for example, an accidental purchase.

`1`  

The App Store refunded the transaction on behalf of the customer due to an actual or perceived issue within your app.

## See Also

### Revocation date and reason

type revocationDate

The UNIX time, in milliseconds, that the App Store refunded the transaction or revoked it from Family Sharing.

