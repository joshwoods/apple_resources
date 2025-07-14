

- Enterprise Program API
-  Invite a User 

Web Service Endpoint

# Invite a User

Invite a user with assigned user roles to join your team.

## URL

``` source
POST https://api.enterprise.developer.apple.com/v1/userInvitations
```

## HTTP Body

UserInvitationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

UserInvitationResponse

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

## Overview

- HTTPBody

## See Also

### Sending and Canceling Invitations

Cancel a User Invitation

Cancel a pending invitation for a user to join your team.

