

- App Store Connect API
-  Add Builds to a Beta Group 

Web Service Endpoint

# Add Builds to a Beta Group

Associate builds with a beta group to enable the group to test the builds.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaGroups/{id}/relationships/builds
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

BetaGroupBuildsLinkagesRequest

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

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

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Adding and Removing Builds and Testers

Add Beta Testers to a Beta Group

Add a specific beta tester to one or more beta groups for beta testing.

Remove Beta Testers from a Beta Group

Remove a specific beta tester from a one or more beta groups, revoking their access to test builds associated with those groups.

Remove Builds from a Beta Group

Remove access to test one or more builds from beta testers in a specific beta group.

