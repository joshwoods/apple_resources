

- App Store Connect API
- AppClipDefaultExperienceCreateRequest
- 
  - AppClipDefaultExperienceCreateRequest
- AppClipDefaultExperienceCreateRequest.Data
- AppClipDefaultExperienceCreateRequest.Data.Relationships
- AppClipDefaultExperienceCreateRequest.Data.Relationships.AppClip
-  AppClipDefaultExperienceCreateRequest.Data.Relationships.AppClip.Data 

Object

# AppClipDefaultExperienceCreateRequest.Data.Relationships.AppClip.Data

The type and ID of the App Clips resource that you’re relating with the Default App Clip Experiences resource you’re creating.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperienceCreateRequest.Data.Relationships.AppClip.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies an App Clips resource.

`type`

`string`

 (Required) 

The resource type.

Value: `appClips`

