

- App Store Connect API
- AppClipDefaultExperienceUpdateRequest
-  AppClipDefaultExperienceUpdateRequest.Data 

Object

# AppClipDefaultExperienceUpdateRequest.Data

The data element of the request body.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperienceUpdateRequest.Data
```

## Properties

`attributes`

AppClipDefaultExperienceUpdateRequest.Data.Attributes

The attributes that describe the request that updates a Default App Clip Experiences resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the request.

`relationships`

AppClipDefaultExperienceUpdateRequest.Data.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipDefaultExperiences`

## Topics

### Objects

object AppClipDefaultExperienceUpdateRequest.Data.Attributes

The attributes you set that describe the new Default App Clip Experiences resource.

object AppClipDefaultExperienceUpdateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

