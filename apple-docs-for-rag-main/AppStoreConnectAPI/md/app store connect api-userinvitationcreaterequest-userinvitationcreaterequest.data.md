

- App Store Connect API
- UserInvitationCreateRequest
-  UserInvitationCreateRequest.Data 

Object

# UserInvitationCreateRequest.Data

The data element of the request body.

App Store Connect API 1.0+

``` source
object UserInvitationCreateRequest.Data
```

## Properties

`attributes`

UserInvitationCreateRequest.Data.Attributes

 (Required) 

The resource’s attributes.

`relationships`

UserInvitationCreateRequest.Data.Relationships

The types and IDs of the related data to update.

`type`

`string`

 (Required) 

The resource type.

Value: `userInvitations`

## Topics

### Objects

object UserInvitationCreateRequest.Data.Attributes

Attributes that you set that describe the new resource.

object UserInvitationCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

