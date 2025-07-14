

- App Store Server API
-  transactionId 

Type

# transactionId

The unique identifier for a transaction, such as an In-App Purchase, restored In-App Purchase, or subscription renewal.

App Store Server API 1.0+

``` source
string transactionId
```

## Mentioned in 

App Store Server API changelog

## Discussion

In a purchase transaction, the `transactionId` matches the original transaction identifier, originalTransactionId. When a customer restores a purchase or renews a subscription, the `transactionId` differs.

## See Also

### Transaction identifiers

type originalTransactionId

The original transaction identifier of a purchase.

type webOrderLineItemId

The unique identifier of subscription-purchase events across devices, including renewals.

