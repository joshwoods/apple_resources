

- App Store Connect API
-  CiMacOsVersionResponse 

Object

# CiMacOsVersionResponse

A response that contains a single macOS Versions resource.

App Store Connect API 1.5+

``` source
object CiMacOsVersionResponse
```

## Properties

`data`

CiMacOsVersion

 (Required) 

The resource data.

`included`

`[`CiXcodeVersion`]`

The requested relationship data.

`links`

DocumentLinks

 (Required) 

The navigational links that include the self-link.

## See Also

### Objects

object CiMacOsVersion

The data structure that represents a macOS Versions resource.

object CiMacOsVersionsResponse

A response that contains a list of macOS Versions resources.

