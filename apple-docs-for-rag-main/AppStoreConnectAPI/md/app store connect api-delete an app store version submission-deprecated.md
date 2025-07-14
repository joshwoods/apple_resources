

- App Store Connect API
-  Delete an App Store Version Submission Deprecated

Web Service Endpoint

# Delete an App Store Version Submission

Remove a version from App Store review.

App Store Connect API 1.2–1.7Deprecated

Deprecated

Use Modify a review submission instead.

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appStoreVersionSubmissions/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier of the App Store version submission resource that you receive when you create the submission. This value is the same as the `id` property in the AppStoreVersionSubmission object.

## Response Codes

` 204 ``No Content`

`No Content`

Success.

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

## Mentioned in 

App Store Connect API 1.7 release notes

## Discussion

Use this endpoint to remove a version from App Review. This request fails with an appropriate error if the app can’t be removed from review. For more information, see Remove a submission from review.

### Remove a Version from App Review

- Request
- Response

```
DELETE https://api.appstoreconnect.apple.com/v1/appStoreVersionSubmissions/942c7a69-b184-478a-898f-a51b8be1044d
```

```
HTTP/1.1 204 NO CONTENT
```

## See Also

### Managing Review Submissions

Create an App Store version submission

Submit an App Store version to App Review.

Deprecated

