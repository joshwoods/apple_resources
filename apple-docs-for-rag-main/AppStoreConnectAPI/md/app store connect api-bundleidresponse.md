

- App Store Connect API
-  BundleIdResponse 

Object

# BundleIdResponse

A response that contains a single Bundle IDs resource.

App Store Connect API 1.1+

``` source
object BundleIdResponse
```

## Properties

`data`

BundleId

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[*]`

The requested relationship data.

Possible types: Profile`, `BundleIdCapability`, `App

## See Also

### Objects and Types

object BundleId

The data structure that represents a Bundle IDs resource.

type BundleIdPlatform

Strings that represent the operating system intended for the bundle.

object BundleIdCreateRequest

The request body you use to create a Bundle ID.

object BundleIdUpdateRequest

The request body you use to update a Bundle ID.

object BundleIdWithoutIncludesResponse

object BundleIdsResponse

A response that contains a list of Bundle ID resources.

