

- App Store Server Notifications
-  originalTransactionId 

Type

# originalTransactionId

The original transaction identifier of a purchase.

App Store Server Notifications 2.0+

``` source
string originalTransactionId
```

## Discussion

This value is identical to the transaction identifier (transactionId) except when the user restores or renews a subscription.

## See Also

### Transaction identifiers

type transactionId

The unique identifier for a transaction, such as an In-App Purchase, restored purchase, or subscription renewal.

type webOrderLineItemId

The unique identifier of subscription purchase events across devices, including subscription renewals.

type previousOriginalTransactionId

The original transaction identifer of a subscription before migration.

