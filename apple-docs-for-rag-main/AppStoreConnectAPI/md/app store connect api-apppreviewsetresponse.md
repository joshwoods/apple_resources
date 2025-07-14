

- App Store Connect API
-  AppPreviewSetResponse 

Object

# AppPreviewSetResponse

A response that contains a single App Preview Sets resource.

App Store Connect API 1.2+

``` source
object AppPreviewSetResponse
```

## Properties

`data`

AppPreviewSet

 (Required) 

`included`

`[*]`

Possible types: AppStoreVersionLocalization`, `AppCustomProductPageLocalization`, `AppStoreVersionExperimentTreatmentLocalization`, `AppPreview

`links`

DocumentLinks

 (Required) 

## See Also

### Objects

object AppPreviewSet

The data structure that represent an App Preview Sets resource.

object AppPreviewSetCreateRequest

The request body you use to create an App Preview Set.

object AppPreviewSetsResponse

A response that contains a list of App Preview Set resources.

object AppPreviewSetAppPreviewsLinkagesRequest

A request body you use to reorder the app previews in a preview set.

object AppPreviewSetAppPreviewsLinkagesResponse

A response body that contains a list of related resource IDs.

