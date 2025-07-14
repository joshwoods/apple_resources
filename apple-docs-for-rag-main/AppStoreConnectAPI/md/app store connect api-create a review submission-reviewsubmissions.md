

- App Store Connect API
-  Create a review submission 

Web Service Endpoint

# Create a review submission

Create a review submission for a specific app.

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/reviewSubmissions
```

## HTTP Body

ReviewSubmissionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

ReviewSubmissionResponse

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

### Endpoints

List review submissions for an app

List recent and current review submissions for a specific app.

Read review submission information

Read information about a specific review submisison.

List the items in a review submission

List all the items in a specific review submission.

Modify a review submission

Edit the details or contents of a review submission.

