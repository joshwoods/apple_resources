

- External Purchase Server API
-  referenceLineItemId 

Type

# referenceLineItemId

The line item identifier of another transaction, that the report references.

External Purchase Server API 1.0.0+

``` source
string referenceLineItemId
```

## Discussion

Maximum length: 128

Use the `referenceLineItemId` field when reporting a transaction that needs to reference a previous transaction.

You report a transaction as a line item, which has a unique lineItemId. Use the original `lineItemId` as the `referenceLineItemId` to report the following types of new transactions:

- Refunds, which refer to the original transaction to which the refund applies

- Subscription events such as renewals, which refer to the initial buy transaction.

Line items include OneTimeBuyLineItem,RefundLineItem, and SubscriptionBuyLineItem.

A referenceLineItemId is valid when it references a line item in the same report, or in a report you previously submitted, successfully.

## See Also

### Providing transaction info

type creationDate

The UNIX date, in milliseconds, that the customer authorized the transaction.

type eventType

The type of transaction the line item reports, whether it’s a buy or refund.

