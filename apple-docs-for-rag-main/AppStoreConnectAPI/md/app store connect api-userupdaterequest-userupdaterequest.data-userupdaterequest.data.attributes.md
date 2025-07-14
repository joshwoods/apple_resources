

- App Store Connect API
- UserUpdateRequest
- UserUpdateRequest.Data
-  UserUpdateRequest.Data.Attributes 

Object

# UserUpdateRequest.Data.Attributes

Attributes whose values you’re changing as part of the update request.

App Store Connect API 1.0+

``` source
object UserUpdateRequest.Data.Attributes
```

## Properties

`allAppsVisible`

`boolean`

Assigned user roles that determine the user’s access to sections of App Store Connect and tasks they can perform.

`provisioningAllowed`

`boolean`

A Boolean value that indicates the user’s specified role allows access to the provisioning functionality on the Apple Developer website.

`roles`

`[`UserRole`]`

Assigned user roles that determine the user’s access to sections of App Store Connect and tasks they can perform.

## See Also

### Related Documentation

Users

Manage users on your App Store Connect team.

### Objects

object UserUpdateRequest.Data.Relationships

The data and links that describe the relationship between the resources.

