

- App Store Connect API
- AppClipAdvancedExperienceCreateRequest
-  AppClipAdvancedExperienceCreateRequest.Data 

Object

# AppClipAdvancedExperienceCreateRequest.Data

The data element of the request body.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperienceCreateRequest.Data
```

## Properties

`attributes`

AppClipAdvancedExperienceCreateRequest.Data.Attributes

 (Required) 

The attributes that describe the request that creates an Advanced App Clip Experiences resource.

`relationships`

AppClipAdvancedExperienceCreateRequest.Data.Relationships

 (Required) 

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipAdvancedExperiences`

## Topics

### Objects

object AppClipAdvancedExperienceCreateRequest.Data.Attributes

The attributes you set that describe the new Advanced App Clip Experiences resource.

object AppClipAdvancedExperienceCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

## See Also

### Objects

object AppClipAdvancedExperienceLocalizationInlineCreate

The data structure that represents an Advanced App Clip Experience Localization Inline Creates resource.

