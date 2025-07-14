

- App Store Connect API
-  UsersResponse 

Object

# UsersResponse

A response that contains a list of Users resources.

App Store Connect API 1.0+

``` source
object UsersResponse
```

## Properties

`data`

`[`User`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

`included`

`[`App`]`

## See Also

### Related Documentation

List Users

Get a list of the users on your team.

### Objects and Data Types

object User

The data structure that represents a Users resource.

object UserUpdateRequest

The request body you use to update a User.

object UserResponse

A response that contains a single Users resource.

object UserVisibleAppsLinkagesRequest

A request body you use to add or remove visible apps from a user.

object UserVisibleAppsLinkagesResponse

A response body that contains a list of related resource IDs.

type UserRole

Strings that represent user roles and permissions in App Store Connect.

