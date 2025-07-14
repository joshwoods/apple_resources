

- External Purchase Server API
-  Send External Purchase Report 

Web Service Endpoint

# Send External Purchase Report

Report required information about external purchase tokens and associated transactions.

External Purchase Server API 1.0.0+

## URL

``` source
PUT https://api.storekit.apple.com/externalPurchase/v1/reports
```

## Sandbox URL

``` source
PUT https://api.storekit-sandbox.apple.com/externalPurchase/v1/reports
```

## HTTP Body

ExternalPurchaseReport

The request body that contains the report information.

Content-Type: application/json

## Response Codes

` 200 ``OK`

SendReportSuccessResponse

`OK`

The report was received and passed validation checks successfully.

Content-Type: application/json

` 400 ``Bad Request`

SendReportErrorResponse

`Bad Request`

The report failed because the request was malformed, a duplicate request, or if the SendReportErrorResponse object is present that the line item validation failed.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid.

` 429 `

` 500 ``Internal Server Error`

`Internal Server Error`

Server error. Try again later.

## Mentioned in 

Reporting corrections

Reporting unrecognized tokens and tokens without transactions

Reporting tokens with transactions

## Discussion

Call this endpoint to report an external purchase token that your app or website receives, and the transactions and events associated with the token. For information on the reporting requirements, see the Commission, transaction reports, and payments section of the article Using alternative payment options on the App Store in the European Union.

To send the report, add your data to the ExternalPurchaseReport request body. For more information about creating reports, see the following:

- Reporting tokens with transactions

- Reporting unrecognized tokens and tokens without transactions

- Reporting corrections

The server indicates it successfully received your report by returning an `HTTP 200` response with your requestIdentifier in the SendReportSuccessResponse. If you receive an `HTTP 400` error response with a SendReportErrorResponse object, the server didn’t successfully receive any of the data in the report. Fix the errors listed in the response object, and resubmit the full report using the same requestIdentifier. The server also sends an `HTTP 400` error if the request is a duplicate, or if it’s malformed.

### Testing in the sandbox environment

Call this endpoint using its sandbox URL only for tokens that the system generates in the sandbox environment. For more information about identifying sandbox tokens, see Receiving and decoding external purchase tokens.

Important

The sandbox tokens and any test transaction data you submit through the sandbox URLs of the External Purchase Server API are not actual transactions.

## See Also

### External purchase reporting

object ExternalPurchaseReport

The contents of an external purchase report for a single token.

object SendReportSuccessResponse

A response that contains the request identifier and indicates the server successfully received your external purchase report.

object SendReportErrorResponse

An error response that indicates your external purchase report didn’t succeed, including error details for the line items in your report.

