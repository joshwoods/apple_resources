

- App Store Connect API
-  User 

Object

# User

The data structure that represents a Users resource.

App Store Connect API 1.0+

``` source
object User
```

## Properties

`attributes`

User.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

User.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `users`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object User.Attributes

Attributes that describe a Users resource.

object User.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Related Documentation

Users

Manage users on your App Store Connect team.

### Objects and Data Types

object UserUpdateRequest

The request body you use to update a User.

object UserResponse

A response that contains a single Users resource.

object UsersResponse

A response that contains a list of Users resources.

object UserVisibleAppsLinkagesRequest

A request body you use to add or remove visible apps from a user.

object UserVisibleAppsLinkagesResponse

A response body that contains a list of related resource IDs.

type UserRole

Strings that represent user roles and permissions in App Store Connect.

