

- App Store Connect API
- UserInvitation
-  UserInvitation.Attributes 

Object

# UserInvitation.Attributes

Attributes that describe a User Invitations resource.

App Store Connect API 1.0+

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

Assigned user roles that determine the user’s access to sections of App Store Connect and tasks they can perform.

`expirationDate`

`date-time`

The expiration date of the pending invitation.

`provisioningAllowed`

`boolean`

A Boolean value that indicates the user’s specified role allows access to the provisioning functionality on the Apple Developer website.

`allAppsVisible`

`boolean`

A Boolean value that indicates whether a user has access to all apps available to the team.

## See Also

### Related Documentation

User Invitations

Email invitations to join your App Store Connect team.

### Objects

object UserInvitation.Relationships

The relationships you included in the request and those on which you can operate.

