

- App Store Connect API
- AppClipDefaultExperienceCreateRequest
- 
  - AppClipDefaultExperienceCreateRequest
- AppClipDefaultExperienceCreateRequest.Data
- AppClipDefaultExperienceCreateRequest.Data.Relationships
- AppClipDefaultExperienceCreateRequest.Data.Relationships.AppClipDefaultExperienceTemplate
-  AppClipDefaultExperienceCreateRequest.Data.Relationships.AppClipDefaultExperienceTemplate.Data 

Object

# AppClipDefaultExperienceCreateRequest.Data.Relationships.AppClipDefaultExperienceTemplate.Data

The type and ID of the Default App Clip Experience Templates resource that you’re relating with the Default App Clip Experiences resource you’re creating.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperienceCreateRequest.Data.Relationships.AppClipDefaultExperienceTemplate.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Default App Clip Experience Templates resource.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipDefaultExperiences`

