

- Enterprise Program API
-  Read user invitation information 

Web Service Endpoint

# Read user invitation information

Get information about a pending invitation to join your team.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/userInvitations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[userInvitations]`

`[string]`

Fields to return for included related types.

Possible Values: `email, expirationDate, firstName, lastName, roles`

## Response Codes

` 200 ``OK`

UserInvitationResponse

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

### Getting Invited Users

List Invited Users

Get a list of pending invitations to join your team.

