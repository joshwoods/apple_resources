

- App Store Connect API
-  BundleIdsResponse 

Object

# BundleIdsResponse

A response that contains a list of Bundle ID resources.

App Store Connect API 1.1+

``` source
object BundleIdsResponse
```

## Properties

`data`

`[`BundleId`]`

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

`[*]`

The requested relationship data.

Possible types: Profile`, `BundleIdCapability`, `App

## See Also

### Related Documentation

List Bundle IDs

Find and list bundle IDs that are registered to your team.

### Objects and Types

object BundleId

The data structure that represents a Bundle IDs resource.

type BundleIdPlatform

Strings that represent the operating system intended for the bundle.

object BundleIdCreateRequest

The request body you use to create a Bundle ID.

object BundleIdUpdateRequest

The request body you use to update a Bundle ID.

object BundleIdResponse

A response that contains a single Bundle IDs resource.

object BundleIdWithoutIncludesResponse

