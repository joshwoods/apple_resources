

- App Store Connect API
-  UserInvitationResponse 

Object

# UserInvitationResponse

A response that contains a single User Invitations resource.

App Store Connect API 1.0+

``` source
object UserInvitationResponse
```

## Properties

`data`

UserInvitation

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[`App`]`

## See Also

### Related Documentation

Invite a User

Invite a user with assigned user roles to join your team.

### Objects

object UserInvitation

The data structure that represents a User Invitations resource.

object UserInvitationCreateRequest

The request body you use to create a User Invitation.

object UserInvitationsResponse

A response that contains a list of User Invitations resources.

