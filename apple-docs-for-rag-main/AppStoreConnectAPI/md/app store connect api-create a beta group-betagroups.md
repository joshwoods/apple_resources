

- App Store Connect API
-  Create a Beta Group 

Web Service Endpoint

# Create a Beta Group

Create a beta group associated with an app, optionally enabling TestFlight public links.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaGroups
```

## HTTP Body

BetaGroupCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BetaGroupResponse

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

### Creating, Modifying, and Deleting Beta Groups

Modify a Beta Group

Modify a beta group’s metadata, including changing its Testflight public link status.

Delete a Beta Group

Delete a beta group and remove beta tester access to associated builds.

