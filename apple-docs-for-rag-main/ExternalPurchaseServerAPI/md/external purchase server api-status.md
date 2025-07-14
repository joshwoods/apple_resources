

- External Purchase Server API
-  status 

Type

# status

A string value that represents the status of the token and the contents of the external purchase report.

External Purchase Server API 1.0.0+

``` source
string status
```

## Possible Values 

`LINE_ITEM`  

`NO_LINE_ITEM`  

`UNRECOGNIZED_TOKEN`  

## Mentioned in 

Reporting unrecognized tokens and tokens without transactions

## Discussion

Allowed values: `LINE_ITEM`, `NO_LINE_ITEM`, `UNRECOGNIZED_TOKEN`

This value is a property you provide in the ExternalPurchaseReport request body when you call the Send External Purchase Report endpoint. The status indicates whether the token has any associated transactions. Include a status value as follows:

- Use `LINE_ITEM` when your external purchase report includes line items to report transactions.

- Use `NO_LINE_ITEM` to report that your app or website received an external purchase token, but the customer didn’t complete any transactions related to the token.

- Use `UNRECOGNIZED_TOKEN` to report that you’ve received an App Store Server Notification about an external purchase token assigned to your app, but your system doesn’t recognize the token.

## See Also

### Data types

type requestIdentifier

A UUID that uniquely identifies an external purchase report.

type externalPurchaseId

The unique identifier of an external purchase token.

