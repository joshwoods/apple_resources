

- Enterprise Program API
- UserInvitationCreateRequest
- UserInvitationCreateRequest.Data
-  UserInvitationCreateRequest.Data.Attributes 

Object

# UserInvitationCreateRequest.Data.Attributes

Attributes that you set that describe the new resource.

``` source
object UserInvitationCreateRequest.Data.Attributes
```

## Properties

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

`roles`

`[`UserRole`]`

 (Required) 

Assigned user roles that determine the user’s access to sections of the Apple Developer website and tasks they can perform.

## Attributes 

Possible types:

