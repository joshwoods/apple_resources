

- App Store Connect API
-  Add Access for Beta Groups to a Build 

Web Service Endpoint

# Add Access for Beta Groups to a Build

Add or create a beta group to a build to enable testing.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/builds/{id}/relationships/betaGroups
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

BuildBetaGroupsLinkagesRequest

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

### Adding and Removing Build Access

Remove Access for Beta Groups to a Build

Remove access to a specific build for all beta testers in one or more beta groups.

Assign Individual Testers to a Build

Enable a beta tester who is not a part of a beta group to test a build.

Remove Individual Testers from a Build

Remove access to test a specific build from one or more individually assigned testers.

