

- App Store Connect API
-  Remove recruitment criteria 

Web Service Endpoint

# Remove recruitment criteria 

Remove the recruitment criteria for your TestFlight build.

App Store Connect API 3.8+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/betaRecruitmentCriteria/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the beta recruitment criteria resource ID from the Read recruitment criteria for a beta group response.

## Response Codes

` 204 ``No Content`

`No Content`

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

## See Also

### Resending Invitations

Create recruitment criteria

Create new criteria for recruiting testers for your TestFlight build.

Modify recruitment criteria

Update the recruitment criteria for your TestFlight build.

Read recruitment criteria for a beta group

Get the recruitment criteria information for a specific beta group.

Read build compatibilty for a beta group

Get the build compatibilty information for a specific beta group.

Read recruitment criteria options

Get a list of the possible beta recruitment criteria options.

