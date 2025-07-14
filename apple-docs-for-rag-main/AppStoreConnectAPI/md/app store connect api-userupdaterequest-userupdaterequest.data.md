

- App Store Connect API
- UserUpdateRequest
-  UserUpdateRequest.Data 

Object

# UserUpdateRequest.Data

The data element of the request body.

App Store Connect API 1.0+

``` source
object UserUpdateRequest.Data
```

## Properties

`attributes`

UserUpdateRequest.Data.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

UserUpdateRequest.Data.Relationships

The types and IDs of the related data to update.

`type`

`string`

 (Required) 

The resource type.

Value: `users`

## Topics

### Objects

object UserUpdateRequest.Data.Attributes

Attributes whose values you’re changing as part of the update request.

object UserUpdateRequest.Data.Relationships

The data and links that describe the relationship between the resources.

