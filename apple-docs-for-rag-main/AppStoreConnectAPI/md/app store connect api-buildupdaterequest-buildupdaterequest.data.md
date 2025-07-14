

- App Store Connect API
- BuildUpdateRequest
-  BuildUpdateRequest.Data 

Object

# BuildUpdateRequest.Data

The data element of the request body.

App Store Connect API 1.0+

``` source
object BuildUpdateRequest.Data
```

## Properties

`attributes`

BuildUpdateRequest.Data.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

BuildUpdateRequest.Data.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `builds`

## Topics

### Objects

object BuildUpdateRequest.Data.Attributes

Attributes whose values you’re changing as part of the update request.

object BuildUpdateRequest.Data.Relationships

The data and links that describe the relationship between the resources.

