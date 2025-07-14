

- App Store Connect API
- AppInfoUpdateRequest
- 
  - AppInfoUpdateRequest
- AppInfoUpdateRequest.Data
- AppInfoUpdateRequest.Data.Relationships
- AppInfoUpdateRequest.Data.Relationships.SecondaryCategory
-  AppInfoUpdateRequest.Data.Relationships.SecondaryCategory.Data 

Object

# AppInfoUpdateRequest.Data.Relationships.SecondaryCategory.Data

The type and ID of a resource that you’re relating with the resource you’re updating.

App Store Connect API 1.2+

``` source
object AppInfoUpdateRequest.Data.Relationships.SecondaryCategory.Data
```

## Properties

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

`type`

`string`

 (Required) 

The resource type.

Value: `appCategories`

