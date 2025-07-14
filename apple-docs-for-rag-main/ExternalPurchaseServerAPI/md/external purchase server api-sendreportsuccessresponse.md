

- External Purchase Server API
-  SendReportSuccessResponse 

Object

# SendReportSuccessResponse

A response that contains the request identifier and indicates the server successfully received your external purchase report.

External Purchase Server API 1.0.0+

``` source
object SendReportSuccessResponse
```

## Properties

`requestIdentifier`

requestIdentifier

 (Required) 

The UUID that you generated to uniquely identify the report when calling the Send External Purchase Report endpoint.

## Discussion

The Send External Purchase Report endpoint returns this response when the server successfully receives a report that passes validation checks. Record the requestIdentifier in your system. Use the `requestIdentifer` to get the report by sending a request to the Retrieve External Purchase Report endpoint.

## See Also

### External purchase reporting

Send External Purchase Report

Report required information about external purchase tokens and associated transactions.

object ExternalPurchaseReport

The contents of an external purchase report for a single token.

object SendReportErrorResponse

An error response that indicates your external purchase report didn’t succeed, including error details for the line items in your report.

