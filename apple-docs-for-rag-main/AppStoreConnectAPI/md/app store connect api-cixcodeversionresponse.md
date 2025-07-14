

- App Store Connect API
-  CiXcodeVersionResponse 

Object

# CiXcodeVersionResponse

A response that contains a single Xcode Versions resource.

App Store Connect API 1.5+

``` source
object CiXcodeVersionResponse
```

## Properties

`data`

CiXcodeVersion

 (Required) 

The resource data.

`included`

`[`CiMacOsVersion`]`

The requested relationship data.

`links`

DocumentLinks

 (Required) 

The navigational links that include the self-link.

## See Also

### Objects

object CiXcodeVersion

The data structure that represents an Xcode Versions resource.

object CiXcodeVersionsResponse

A response that contains a list of Xcode Versions resources.

