

- App Store Connect API
-  UserInvitationsResponse 

Object

# UserInvitationsResponse

A response that contains a list of User Invitations resources.

App Store Connect API 1.0+

``` source
object UserInvitationsResponse
```

## Properties

`data`

`[`UserInvitation`]`

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

List Invited Users

Get a list of pending invitations to join your team.

### Objects

object UserInvitation

The data structure that represents a User Invitations resource.

object UserInvitationCreateRequest

The request body you use to create a User Invitation.

object UserInvitationResponse

A response that contains a single User Invitations resource.

