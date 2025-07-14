

- App Store Connect API
-  Individually Assign a Beta Tester to Builds 

Web Service Endpoint

# Individually Assign a Beta Tester to Builds

Individually assign a beta tester to a build.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaTesters/{id}/relationships/builds
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

BetaTesterBuildsLinkagesRequest

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

### Assigning Groups and Access

Add a Beta Tester to Beta Groups

Add one or more beta testers to a specific beta group.

Remove a Beta Tester from Beta Groups

Remove a specific beta tester from one or more beta groups, revoking their access to test builds associated with those groups.

Individually Unassign a Beta Tester from Builds

Remove an individually assigned beta tester’s ability to test a build.

Remove a Beta Tester’s Access to Apps

Remove a specific beta tester’s access to test any builds of one or more apps.

