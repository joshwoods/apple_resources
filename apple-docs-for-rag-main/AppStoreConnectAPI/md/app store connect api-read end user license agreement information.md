

- App Store Connect API
-  Read End User License Agreement Information 

Web Service Endpoint

# Read End User License Agreement Information

Get the custom end user license agreement associated with an app, and the territories it applies to.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[endUserLicenseAgreements]`

`[string]`

Possible Values: `agreementText, app, territories`

`fields[territories]`

`[string]`

Value: `currency`

`include`

`[string]`

Possible Values: `app, territories`

`limit[territories]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

EndUserLicenseAgreementResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## See Also

### Reading EULA and Listing Territories

Read the End User License Agreement Information of an App

Get the custom end user license agreement (EULA) for a specific app and the territories where the agreement applies.

List All Territories for an End User License Agreement

List all the App Store territories to which a specific custom app license agreement applies.

