

- App Store Connect API
-  Delete an App Store Review Attachment 

Web Service Endpoint

# Delete an App Store Review Attachment

Remove an attachment before you send your app to App Review.

App Store Connect API 1.2+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appStoreReviewAttachments/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

## See Also

### Creating, Modifying, and Deleting Attachments

Create an App Store Review Attachment

Attach a document for App Review to an App Store version.

Commit an App Store Review Attachment

Commit an app screenshot after uploading it to the App Store.

