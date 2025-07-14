

- External Purchase Server API
-  requestIdentifier 

Type

# requestIdentifier

A UUID that uniquely identifies an external purchase report.

External Purchase Server API 1.0.0+

``` source
uuid requestIdentifier
```

## Mentioned in 

Reporting unrecognized tokens and tokens without transactions

Reporting corrections

## Discussion

You generate this identifier when you send a report to the Send External Purchase Report endpoint. Use the same `requestIdentifier` only if you resubmit a report that previously failed. Use a new `requestIdentifier` for each new report, including for reports that correct line items you previously submitted successfully.

Use the `requestIdentifier` to get the report from the Retrieve External Purchase Report endpoint.

## See Also

### Data types

type externalPurchaseId

The unique identifier of an external purchase token.

type status

A string value that represents the status of the token and the contents of the external purchase report.

