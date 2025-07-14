

- App Store Connect API
-  CiBuildActionsResponse 

Object

# CiBuildActionsResponse

A response that contains a list of Build Actions resources.

App Store Connect API 1.5+

``` source
object CiBuildActionsResponse
```

## Properties

`data`

`[`CiBuildAction`]`

 (Required) 

The resource data.

`included`

`[`CiBuildRun`]`

The requested relationship data.

`links`

PagedDocumentLinks

 (Required) 

The navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## See Also

### Objects

object CiBuildRun

The data structure that represents a Build Runs resource.

object CiBuildRunCreateRequest

The request body you use to start a new Xcode Cloud build.

object CiBuildRunResponse

A response that contains a single Build Runs resource.

