

- App Store Connect API
-  AppClipDefaultExperience 

Object

# AppClipDefaultExperience

The data structure that represents a Default App Clip Experiences resource.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperience
```

## Properties

`attributes`

AppClipDefaultExperience.Attributes

The attributes that describe the Default App Clip Experiences resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Default App Clip Experiences resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

AppClipDefaultExperience.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipDefaultExperiences`

## Topics

### Objects

object AppClipDefaultExperience.Attributes

The attributes that describe a Default App Clip Experiences resource.

object AppClipDefaultExperience.Relationships

The relationships of the Default App Clip Experiences resource you included in the request and those on which you can operate.

## See Also

### Objects and Types

object AppClipDefaultExperienceResponse

A response that contains a single Default App Clip Experiences resource.

object AppClipDefaultExperienceCreateRequest

The request body you use to create a default App Clip experience.

object AppClipDefaultExperienceUpdateRequest

The request body you use to update a default App Clip experience.

object AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest

The request body you use to relate a released App Store version with a default App Clip experience.

object AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse

A response that contains the ID of a single related App Store Versions resource.

type AppClipAction

A string that represents the call- termto- termaction verb on the App Clip card.

