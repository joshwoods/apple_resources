

- App Store Connect API
-  UserVisibleAppsLinkagesResponse 

Object

# UserVisibleAppsLinkagesResponse

A response body that contains a list of related resource IDs.

App Store Connect API 1.0+

``` source
object UserVisibleAppsLinkagesResponse
```

## Properties

`data`

`[`UserVisibleAppsLinkagesResponse.Data`]`

 (Required) 

The object types and IDs of the related resources.

`links`

PagedDocumentLinks

 (Required) 

Navigational links including the self-link and links to the related data.

`meta`

PagingInformation

Paging information.

## Topics

### Objects

object UserVisibleAppsLinkagesResponse.Data

The data element of the response body.

## See Also

### Related Documentation

Get All Visible App Resource IDs for a User

Get a list of app resource IDs to which a user on your team has access.

### Objects and Data Types

object User

The data structure that represents a Users resource.

object UserUpdateRequest

The request body you use to update a User.

object UserResponse

A response that contains a single Users resource.

object UsersResponse

A response that contains a list of Users resources.

object UserVisibleAppsLinkagesRequest

A request body you use to add or remove visible apps from a user.

type UserRole

Strings that represent user roles and permissions in App Store Connect.

