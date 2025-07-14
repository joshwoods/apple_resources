

- App Store Connect API
-  AppClipAdvancedExperience 

Object

# AppClipAdvancedExperience

The data structure that represents an Advanced App Clip Experiences resource.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperience
```

## Properties

`attributes`

AppClipAdvancedExperience.Attributes

The attributes that describe the Advanced App Clip Experiences resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies an Advanced App Clip Experiences resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

AppClipAdvancedExperience.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipAdvancedExperiences`

## Topics

### Objects

object AppClipAdvancedExperience.Attributes

The attributes that describe an Advanced App Clip Experiences resource.

object AppClipAdvancedExperience.Relationships

The relationships of the Advanced App Clip Experiences resource you included in the request and those on which you can operate.

## See Also

### Objects and Types

object AppClipAdvancedExperienceResponse

A response that contains a single Advanced App Clip Experiences resource.

object AppClipAdvancedExperienceLocalization

The data structure that represents the Advanced App Clip Localizations resource.

object AppClipAdvancedExperienceCreateRequest

The request body you use to create an advanced App Clip experience.

object AppClipAdvancedExperienceUpdateRequest

The request body you use to update an advanced App Clip experience.

type AppClipAdvancedExperienceLanguage

The data structure that represents the language you configure for an advanced App Clip experience.

