

- App Store Connect API
-  Create a Beta Tester 

Web Service Endpoint

# Create a Beta Tester

Create a beta tester assigned to a group, a build, or an app.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaTesters
```

## HTTP Body

BetaTesterCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BetaTesterResponse

`Created`

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

## See Also

### Creating and Deleting Beta Testers

Delete a Beta Tester

Remove a beta tester’s ability to test all apps.

