

- App Store Connect API
-  UserInvitation 

Object

# UserInvitation

The data structure that represents a User Invitations resource.

App Store Connect API 1.0+

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

`relationships`

UserInvitation.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `userInvitations`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object UserInvitation.Attributes

Attributes that describe a User Invitations resource.

object UserInvitation.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object UserInvitationCreateRequest

The request body you use to create a User Invitation.

object UserInvitationResponse

A response that contains a single User Invitations resource.

object UserInvitationsResponse

A response that contains a list of User Invitations resources.

