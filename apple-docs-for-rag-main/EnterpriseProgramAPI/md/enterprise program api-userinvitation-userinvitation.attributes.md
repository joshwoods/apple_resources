

- Enterprise Program API
- UserInvitation
-  UserInvitation.Attributes 

Object

# UserInvitation.Attributes

Attributes that describe a User Invitations resource.

``` source
object UserInvitation.Attributes
```

## Properties

`email`

`email`

The email address of a pending user invitation. The email address must be valid to activate the account. It can be any email address, not necessarily one associated with an Apple Account.

`firstName`

`string`

The first name of the user with the pending user invitation.

`lastName`

`string`

The last name of the user with the pending user invitation.

`roles`

`[`UserRole`]`

Assigned user roles that determine the user’s access to sections of the Apple Developer website and tasks they can perform.

`expirationDate`

`date-time`

The expiration date of the pending invitation.

## Attributes 

Possible types:

