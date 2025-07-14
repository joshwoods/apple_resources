

- App Store Connect API
- AppStoreVersionUpdateRequest
- 
  - AppStoreVersionUpdateRequest
- AppStoreVersionUpdateRequest.Data
- AppStoreVersionUpdateRequest.Data.Relationships
- AppStoreVersionUpdateRequest.Data.Relationships.AppClipDefaultExperience
-  AppStoreVersionUpdateRequest.Data.Relationships.AppClipDefaultExperience.Data 

Object

# AppStoreVersionUpdateRequest.Data.Relationships.AppClipDefaultExperience.Data

The type and ID of the Default App Clip Experiences resource that you’re relating with the App Store Versions resource you’re updating.

App Store Connect API 1.6+

``` source
object AppStoreVersionUpdateRequest.Data.Relationships.AppClipDefaultExperience.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Default App Clip Experiences resource.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipDefaultExperiences`

