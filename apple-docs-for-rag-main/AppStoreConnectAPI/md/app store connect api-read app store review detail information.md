

- App Store Connect API
-  Read App Store Review Detail Information 

Web Service Endpoint

# Read App Store Review Detail Information

Get App Review details you provided, including contact information, demo account, and notes.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreReviewDetails/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appStoreReviewDetails]`

`[string]`

Possible Values: `contactFirstName, contactLastName, contactPhone, contactEmail, demoAccountName, demoAccountPassword, demoAccountRequired, notes, appStoreVersion, appStoreReviewAttachments`

`include`

`[string]`

Possible Values: `appStoreVersion, appStoreReviewAttachments`

`limit[appStoreReviewAttachments]`

`integer`

Maximum: `50`

`fields[appStoreReviewAttachments]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, uploadOperations, assetDeliveryState, appStoreReviewDetail`

## Response Codes

` 200 ``OK`

AppStoreReviewDetailResponse

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

### Creating, Modifying, and Reading Review Details

Create an App Store Review Detail

Add App Store review details to an App Store version, including contact and demo account information.

Modify an App Store Review Detail

Update the app store review details, including the contact information, demo account, and notes.

