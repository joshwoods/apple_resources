

- App Store Connect API
-  Create an App Store Review Attachment 

Web Service Endpoint

# Create an App Store Review Attachment

Attach a document for App Review to an App Store version.

App Store Connect API 1.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appStoreReviewAttachments
```

## HTTP Body

AppStoreReviewAttachmentCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreReviewAttachmentResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Creating, Modifying, and Deleting Attachments

Commit an App Store Review Attachment

Commit an app screenshot after uploading it to the App Store.

Delete an App Store Review Attachment

Remove an attachment before you send your app to App Review.

