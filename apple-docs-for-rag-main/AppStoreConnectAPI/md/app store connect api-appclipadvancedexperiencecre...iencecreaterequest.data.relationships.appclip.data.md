

- App Store Connect API
- AppClipAdvancedExperienceCreateRequest
- 
  - AppClipAdvancedExperienceCreateRequest
- AppClipAdvancedExperienceCreateRequest.Data
- AppClipAdvancedExperienceCreateRequest.Data.Relationships
- AppClipAdvancedExperienceCreateRequest.Data.Relationships.AppClip
-  AppClipAdvancedExperienceCreateRequest.Data.Relationships.AppClip.Data 

Object

# AppClipAdvancedExperienceCreateRequest.Data.Relationships.AppClip.Data

The type and ID of the App Clips resource that you’re relating with the Advanced App Clip Experiences resource you’re creating.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperienceCreateRequest.Data.Relationships.AppClip.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related App Clips resource.

`type`

`string`

 (Required) 

The resource type.

Value: `appClips`

