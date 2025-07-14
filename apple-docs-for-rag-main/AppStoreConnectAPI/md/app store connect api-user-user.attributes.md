

- App Store Connect API
- User
-  User.Attributes 

Object

# User.Attributes

Attributes that describe a Users resource.

App Store Connect API 1.0+

``` source
object User.Attributes
```

## Properties

`firstName`

`string`

The user’s first name.

`lastName`

`string`

The user’s last name.

`roles`

`[`UserRole`]`

Assigned user roles that determine the user’s access to sections of App Store Connect and tasks they can perform.

`provisioningAllowed`

`boolean`

A Boolean value that indicates the user’s specified role allows access to the provisioning functionality on the Apple Developer website.

`allAppsVisible`

`boolean`

A Boolean value that indicates whether a user has access to all apps available to the team.

`username`

`string`

The user’s Apple Account.

## See Also

### Related Documentation

Users

Manage users on your App Store Connect team.

### Objects

object User.Relationships

The relationships you included in the request and those on which you can operate.

