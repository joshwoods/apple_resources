

- App Store Connect API
-  AppClipResponse 

Object

# AppClipResponse

A response that contains a single App Clips resource.

App Store Connect API 1.6+

``` source
object AppClipResponse
```

## Properties

`data`

AppClip

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: App`, `AppClipDefaultExperience

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## See Also

### Objects

object AppClip

The data structure that represents an App Clips resource.

object AppClipDefaultExperiencesResponse

A response that contains a list of Default App Clip Experiences resources.

object AppClipAdvancedExperiencesResponse

A response that contains a list of Advanced App Clip Experiences resources.

