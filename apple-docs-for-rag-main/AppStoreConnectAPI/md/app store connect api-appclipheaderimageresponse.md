

- App Store Connect API
-  AppClipHeaderImageResponse 

Object

# AppClipHeaderImageResponse

A response that contains a single App Clip Header Images resource.

App Store Connect API 1.6+

``` source
object AppClipHeaderImageResponse
```

## Properties

`data`

AppClipHeaderImage

 (Required) 

The resource data.

`included`

`[`AppClipDefaultExperienceLocalization`]`

The requested relationship data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## See Also

### Objects

object AppClipHeaderImage

The data structure that represents the image that appears on the App Clip card of a default App Clip experience.

object AppClipHeaderImageCreateRequest

The request body you use to reserve an image asset that appears on the App Clip card of a default App Clip experience.

object AppClipHeaderImageUpdateRequest

The request body you use to commit the image asset for a default App Clip experience.

