

- External Purchase Server API
-  creationDate 

Type

# creationDate

The UNIX date, in milliseconds, that the customer authorized the transaction.

External Purchase Server API 1.0.0+

``` source
int64 creationDate
```

## Discussion

For refunds and other events, use the UNIX date, in milliseconds, of the transaction.

## See Also

### Providing transaction info

type eventType

The type of transaction the line item reports, whether it’s a buy or refund.

type referenceLineItemId

The line item identifier of another transaction, that the report references.

