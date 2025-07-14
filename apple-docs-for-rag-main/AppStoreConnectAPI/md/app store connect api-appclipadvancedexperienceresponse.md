

- App Store Connect API
-  AppClipAdvancedExperienceResponse 

Object

# AppClipAdvancedExperienceResponse

A response that contains a single Advanced App Clip Experiences resource.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperienceResponse
```

## Properties

`data`

AppClipAdvancedExperience

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: AppClip`, `AppClipAdvancedExperienceImage`, `AppClipAdvancedExperienceLocalization

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## See Also

### Objects and Types

object AppClipAdvancedExperience

The data structure that represents an Advanced App Clip Experiences resource.

object AppClipAdvancedExperienceLocalization

The data structure that represents the Advanced App Clip Localizations resource.

object AppClipAdvancedExperienceCreateRequest

The request body you use to create an advanced App Clip experience.

object AppClipAdvancedExperienceUpdateRequest

The request body you use to update an advanced App Clip experience.

type AppClipAdvancedExperienceLanguage

The data structure that represents the language you configure for an advanced App Clip experience.

