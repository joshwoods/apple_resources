

- App Store Connect API
-  BuildBetaDetailResponse 

Object

# BuildBetaDetailResponse

A response that contains a single Build Beta Details resource.

App Store Connect API 1.0+

``` source
object BuildBetaDetailResponse
```

## Properties

`data`

BuildBetaDetail

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[`Build`]`

## See Also

### Related Documentation

Read Build Beta Detail Information

Get a specific build beta details resource.

### Objects and Data Types

object BuildBetaDetail

The data structure that represents a Build Beta Details resource.

object BuildBetaDetailUpdateRequest

The request body you use to update a Build Data Detail.

object BuildBetaDetailsResponse

A response that contains a list of Build Beta Detail resources.

type ExternalBetaState

String that represents a build’s availability for external testing.

type InternalBetaState

String that represents a build’s availability for internal testing.

