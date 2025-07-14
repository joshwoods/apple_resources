

- App Store Connect API
-  Read App Store Review Attachment Information 

Web Service Endpoint

# Read App Store Review Attachment Information

Get information about an App Store review attachment and its upload and processing status.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreReviewAttachments/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appStoreReviewAttachments]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, uploadOperations, assetDeliveryState, appStoreReviewDetail`

`include`

`[string]`

Value: `appStoreReviewDetail`

## Response Codes

` 200 ``OK`

AppStoreReviewAttachmentResponse

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

List All Review Attachments for an App Store Review Detail

List all the App Store review attachments you include with a version when you submit it for App Review.

