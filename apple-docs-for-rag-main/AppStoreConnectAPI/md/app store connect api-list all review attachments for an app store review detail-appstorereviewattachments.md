

- App Store Connect API
-  List All Review Attachments for an App Store Review Detail 

Web Service Endpoint

# List All Review Attachments for an App Store Review Detail

List all the App Store review attachments you include with a version when you submit it for App Review.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreReviewDetails/{id}/appStoreReviewAttachments
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appStoreReviewAttachments]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, uploadOperations, assetDeliveryState, appStoreReviewDetail`

`limit`

`integer`

Maximum: `200`

`fields[appStoreReviewDetails]`

`[string]`

Possible Values: `contactFirstName, contactLastName, contactPhone, contactEmail, demoAccountName, demoAccountPassword, demoAccountRequired, notes, appStoreVersion, appStoreReviewAttachments`

`include`

`[string]`

Value: `appStoreReviewDetail`

## Response Codes

` 200 ``OK`

AppStoreReviewAttachmentsResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Reading Attachment Information

Read App Store Review Attachment Information

Get information about an App Store review attachment and its upload and processing status.

