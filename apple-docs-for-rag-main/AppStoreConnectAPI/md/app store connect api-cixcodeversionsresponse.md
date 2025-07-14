

- App Store Connect API
-  CiXcodeVersionsResponse 

Object

# CiXcodeVersionsResponse

A response that contains a list of Xcode Versions resources.

App Store Connect API 1.5+

``` source
object CiXcodeVersionsResponse
```

## Properties

`data`

`[`CiXcodeVersion`]`

 (Required) 

The resource data.

`included`

`[`CiMacOsVersion`]`

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

object CiXcodeVersion

The data structure that represents an Xcode Versions resource.

object CiXcodeVersionResponse

A response that contains a single Xcode Versions resource.

