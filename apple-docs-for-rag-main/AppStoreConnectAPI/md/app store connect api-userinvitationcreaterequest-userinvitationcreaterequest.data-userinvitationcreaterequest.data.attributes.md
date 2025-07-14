

- App Store Connect API
- UserInvitationCreateRequest
- UserInvitationCreateRequest.Data
-  UserInvitationCreateRequest.Data.Attributes 

Object

# UserInvitationCreateRequest.Data.Attributes

Attributes that you set that describe the new resource.

App Store Connect API 1.0+

``` source
object UserInvitationCreateRequest.Data.Attributes
```

## Properties

`allAppsVisible`

`boolean`

A Boolean value that indicates whether a user has access to all apps available to the team.

`email`

`email`

 (Required) 

The email address of a pending user invitation. The email address must be valid to activate the account. It can be any email address, not necessarily one associated with an Apple Account.

`firstName`

`string`

 (Required) 

The user invitation recipient’s first name.

`lastName`

`string`

 (Required) 

The user invitation recipient’s last name.

`provisioningAllowed`

`boolean`

A Boolean value that indicates the user’s specified role allows access to the provisioning functionality on the Apple Developer website.

`roles`

`[`UserRole`]`

 (Required) 

Assigned user roles that determine the user’s access to sections of App Store Connect and tasks they can perform.

## See Also

### Related Documentation

User Invitations

Email invitations to join your App Store Connect team.

### Objects

object UserInvitationCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

