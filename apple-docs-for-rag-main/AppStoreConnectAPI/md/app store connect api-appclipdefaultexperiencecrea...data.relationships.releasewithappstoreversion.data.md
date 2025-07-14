

- App Store Connect API
- AppClipDefaultExperienceCreateRequest
- 
  - AppClipDefaultExperienceCreateRequest
- AppClipDefaultExperienceCreateRequest.Data
- AppClipDefaultExperienceCreateRequest.Data.Relationships
- AppClipDefaultExperienceCreateRequest.Data.Relationships.ReleaseWithAppStoreVersion
-  AppClipDefaultExperienceCreateRequest.Data.Relationships.ReleaseWithAppStoreVersion.Data 

Object

# AppClipDefaultExperienceCreateRequest.Data.Relationships.ReleaseWithAppStoreVersion.Data

The type and ID of the App Store Versions resource that you’re relating with the Default App Clip Experiences resource you’re creating.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperienceCreateRequest.Data.Relationships.ReleaseWithAppStoreVersion.Data
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

