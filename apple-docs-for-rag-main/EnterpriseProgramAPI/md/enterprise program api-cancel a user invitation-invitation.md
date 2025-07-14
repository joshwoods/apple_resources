

- Enterprise Program API
-  Cancel a User Invitation 

Web Service Endpoint

# Cancel a User Invitation

Cancel a pending invitation for a user to join your team.

## URL

``` source
DELETE https://api.enterprise.developer.apple.com/v1/userInvitations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Sending and Canceling Invitations

Invite a User

Invite a user with assigned user roles to join your team.

