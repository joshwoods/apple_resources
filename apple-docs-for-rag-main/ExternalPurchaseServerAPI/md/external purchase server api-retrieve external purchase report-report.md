

- External Purchase Server API
-  Retrieve External Purchase Report 

Web Service Endpoint

# Retrieve External Purchase Report

Get an external purchase report by providing its request identifier.

External Purchase Server API 1.0.0+

## URL

``` source
GET https://api.storekit.apple.com/externalPurchase/v1/reports/{requestIdentifier}
```

## Sandbox URL

``` source
GET https://api.storekit-sandbox.apple.com/externalPurchase/v1/reports/{requestIdentifier}
```

## Path Parameters

`requestIdentifier`

requestIdentifier

 (Required) 

The UUID that identifies the external purchase report you’re requesting.

## Response Codes

` 200 ``OK`

RetrieveReportSuccessResponse

`OK`

Success. The RetrieveReportSuccessResponse object contains your report.

Content-Type: application/json

` 400 ``Bad Request`

NotFoundError

`Bad Request`

The request returned an error. Check the `requestIdentifier` parameter to ensure it’s a valid identifer for a report that you successfully submitted.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid.

` 429 `

` 500 ``Internal Server Error`

`Internal Server Error`

Server error. Try again later.

## Discussion

Call this endpoint to retrieve an external purchase report that you successfully sent to Apple. This endpoint takes the `requestIdentifier` that you create when you call Send External Purchase Report, for reports that were successfully submitted.

## Topics

### Data types

type requestIdentifier

A UUID that uniquely identifies an external purchase report.

## See Also

### External purchase report retrieval

object RetrieveReportSuccessResponse

A response that indicates success and includes your external purchase report data.

