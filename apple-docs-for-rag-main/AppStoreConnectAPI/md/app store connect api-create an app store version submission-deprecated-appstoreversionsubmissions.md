

- App Store Connect API
-  Create an App Store version submission Deprecated

Web Service Endpoint

# Create an App Store version submission

Submit an App Store version to App Review.

App Store Connect API 1.2–1.7Deprecated

Deprecated

Use Create a review submission instead.

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appStoreVersionSubmissions
```

## HTTP Body

AppStoreVersionSubmissionCreateRequest

The request body.

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreVersionSubmissionResponse

`Created`

Success.

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Mentioned in 

App Store Connect API 1.7 release notes

## Discussion

Use this endpoint to submit a version to the App Store. If the version is missing required information, this request fails and the response contains error messages that indicate the problems.

If the version’s `releaseType` attribute is `AFTER_APPROVAL`, after App Review approves the version App Store Connect automatically releases it to the App Store.

### Submit a Version to the App Store

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/appStoreVersionSubmissions

{
  "data": {
    "type": "appStoreVersionSubmissions",
    "relationships": {
      "appStoreVersion": {
        "data": {
          "type": "appStoreVersions",
          "id": "54457681-4b65-4071-a636-ea66cb98c8e9"
        }
      }
    }
  }
}

```

```
{
  "data": {
    "type": "appStoreVersionSubmissions",
    "id": "942c7a69-b184-478a-898f-a51b8be1044d",
    "attributes": {
        "canReject": true
    },
    "relationships": {
      "appStoreVersion": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersionSubmissions/942c7a69-b184-478a-898f-a51b8be1044d/relationships/appStoreVersion",
          "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersionSubmissions/942c7a69-b184-478a-898f-a51b8be1044d/appStoreVersion"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersionSubmissions/942c7a69-b184-478a-898f-a51b8be1044d"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersionSubmissions"
  }
}
```

## See Also

### Managing Review Submissions

Delete an App Store Version Submission

Remove a version from App Store review.

Deprecated

