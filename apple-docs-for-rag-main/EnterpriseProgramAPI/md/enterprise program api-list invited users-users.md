

- Enterprise Program API
-  List Invited Users 

Web Service Endpoint

# List Invited Users

Get a list of pending invitations to join your team.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/userInvitations
```

## Query Parameters

`fields[userInvitations]`

`[string]`

Fields to return for included related types.

Possible Values: `email, expirationDate, firstName, lastName, roles`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`sort`

`[string]`

Attributes by which to sort.

Possible Values: `email, -email, lastName, -lastName`

`filter[roles]`

`[string]`

Attributes, relationships, and IDs by which to filter.

Possible Values: `ADMIN, ACCOUNT_HOLDER, DEVELOPER`

`filter[email]`

`[string]`

Attributes, relationships, and IDs by which to filter.

## Response Codes

` 200 ``OK`

UserInvitationsResponse

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

## See Also

### Getting Invited Users

Read user invitation information

Get information about a pending invitation to join your team.

