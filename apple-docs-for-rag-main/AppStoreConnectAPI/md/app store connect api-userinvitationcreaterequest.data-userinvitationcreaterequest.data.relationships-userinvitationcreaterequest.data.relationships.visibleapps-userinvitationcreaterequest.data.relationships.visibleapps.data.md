

- App Store Connect API
- UserInvitationCreateRequest
- 
  - UserInvitationCreateRequest
- UserInvitationCreateRequest.Data
- UserInvitationCreateRequest.Data.Relationships
- UserInvitationCreateRequest.Data.Relationships.VisibleApps
-  UserInvitationCreateRequest.Data.Relationships.VisibleApps.Data 

Object

# UserInvitationCreateRequest.Data.Relationships.VisibleApps.Data

The type and ID of the resource that you’re relating with the resource you’re creating.

App Store Connect API 1.0+

``` source
object UserInvitationCreateRequest.Data.Relationships.VisibleApps.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`type`

`string`

 (Required) 

The resource type.

Value: `apps`

