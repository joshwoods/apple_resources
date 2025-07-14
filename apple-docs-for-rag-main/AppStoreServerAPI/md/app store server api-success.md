

- App Store Server API
-  success 

Type

# success

A Boolean value that indicates whether the subscription-renewal-date extension succeeded.

App Store Server API 1.1+

``` source
boolean success
```

## Discussion

If this value is `true`, the renewal date for the subscription is extended.

## See Also

### Response data types

type effectiveDate

The new subscription expiration date for a subscription-renewal extension.

type originalTransactionId

The original transaction identifier of a purchase.

type webOrderLineItemId

The unique identifier of subscription-purchase events across devices, including renewals.

