

- App Store Connect API
- AppClipDefaultExperienceUpdateRequest
- 
  - AppClipDefaultExperienceUpdateRequest
- AppClipDefaultExperienceUpdateRequest.Data
- AppClipDefaultExperienceUpdateRequest.Data.Relationships
- AppClipDefaultExperienceUpdateRequest.Data.Relationships.ReleaseWithAppStoreVersion
-  AppClipDefaultExperienceUpdateRequest.Data.Relationships.ReleaseWithAppStoreVersion.Data 

Object

# AppClipDefaultExperienceUpdateRequest.Data.Relationships.ReleaseWithAppStoreVersion.Data

The type and ID of the App Store Versions resource that you’re relating with the Default App Clip Experiences resource you’re updating.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperienceUpdateRequest.Data.Relationships.ReleaseWithAppStoreVersion.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related App Store Versions resource.

`type`

`string`

 (Required) 

The resource type.

Value: `appStoreVersions`

