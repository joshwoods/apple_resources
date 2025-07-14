

- App Store Connect API
-  BuildBetaDetailsResponse 

Object

# BuildBetaDetailsResponse

A response that contains a list of Build Beta Detail resources.

App Store Connect API 1.0+

``` source
object BuildBetaDetailsResponse
```

## Properties

`data`

`[`BuildBetaDetail`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

`included`

`[`Build`]`

## See Also

### Related Documentation

List Build Beta Details

Find and list build beta details for all builds.

### Objects and Data Types

object BuildBetaDetail

The data structure that represents a Build Beta Details resource.

object BuildBetaDetailUpdateRequest

The request body you use to update a Build Data Detail.

object BuildBetaDetailResponse

A response that contains a single Build Beta Details resource.

type ExternalBetaState

String that represents a build’s availability for external testing.

type InternalBetaState

String that represents a build’s availability for internal testing.

