

- App Store Connect API
-  CiMacOsVersionsResponse 

Object

# CiMacOsVersionsResponse

A response that contains a list of macOS Versions resources.

App Store Connect API 1.5+

``` source
object CiMacOsVersionsResponse
```

## Properties

`data`

`[`CiMacOsVersion`]`

 (Required) 

The resource data.

`included`

`[`CiXcodeVersion`]`

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

object CiMacOsVersion

The data structure that represents a macOS Versions resource.

object CiMacOsVersionResponse

A response that contains a single macOS Versions resource.

