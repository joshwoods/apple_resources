

- Enterprise Program API
-  UserInvitation 

Object

# UserInvitation

The data structure that represents a User Invitations resource.

``` source
object UserInvitation
```

## Properties

`attributes`

UserInvitation.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`type`

`string`

 (Required) 

The resource type.

Value: `userInvitations`

`links`

ResourceLinks

Navigational links that include the self-link.

## Attributes 

Possible types:

## Topics

### Objects

object UserInvitation.Attributes

Attributes that describe a User Invitations resource.

## See Also

### Objects

object UserInvitationCreateRequest

The request body you use to create a User Invitation.

object UserInvitationResponse

A response that contains a single User Invitations resource.

object UserInvitationsResponse

A response that contains a list of User Invitations resources.

