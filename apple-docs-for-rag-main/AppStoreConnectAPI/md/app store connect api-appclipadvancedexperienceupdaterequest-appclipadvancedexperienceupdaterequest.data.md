

- App Store Connect API
- AppClipAdvancedExperienceUpdateRequest
-  AppClipAdvancedExperienceUpdateRequest.Data 

Object

# AppClipAdvancedExperienceUpdateRequest.Data

The data element of the request body.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperienceUpdateRequest.Data
```

## Properties

`attributes`

AppClipAdvancedExperienceUpdateRequest.Data.Attributes

The attributes that describe the request that updates an Advanced App Clip Experiences resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the request.

`relationships`

AppClipAdvancedExperienceUpdateRequest.Data.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipAdvancedExperiences`

## Topics

### Objects

object AppClipAdvancedExperienceUpdateRequest.Data.Attributes

The attributes you set that describe the Advanced App Clip Experiences resource.

object AppClipAdvancedExperienceUpdateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

