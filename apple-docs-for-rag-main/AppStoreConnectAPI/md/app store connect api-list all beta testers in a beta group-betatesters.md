

- App Store Connect API
-  List All Beta Testers in a Beta Group 

Web Service Endpoint

# List All Beta Testers in a Beta Group

Get a list of beta testers contained in a specific beta group.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaGroups/{id}/betaTesters
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`fields[betaTesters]`

`[string]`

Fields to return for included related types.

Possible Values: `firstName, lastName, email, inviteType, state, apps, betaGroups, builds`

## Response Codes

` 200 ``OK`

BetaTestersWithoutIncludesResponse

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

### Reading Build and Beta Tester Information

List All Builds for a Beta Group

Get a list of builds associated with a specific beta group.

Get All Build IDs in a Beta Group

Get a list of build resource IDs in a specific beta group.

Get All Beta Tester IDs in a Beta Group

Get a list of the beta tester resource IDs in a specific beta group.

