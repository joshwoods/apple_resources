

- App Store Connect API
-  UserResponse 

Object

# UserResponse

A response that contains a single Users resource.

App Store Connect API 1.0+

``` source
object UserResponse
```

## Properties

`data`

User

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

Read User Information

Get information about a user on your team, such as name, roles, and app visibility.

### Objects and Data Types

object User

The data structure that represents a Users resource.

object UserUpdateRequest

The request body you use to update a User.

object UsersResponse

A response that contains a list of Users resources.

object UserVisibleAppsLinkagesRequest

A request body you use to add or remove visible apps from a user.

object UserVisibleAppsLinkagesResponse

A response body that contains a list of related resource IDs.

type UserRole

Strings that represent user roles and permissions in App Store Connect.

