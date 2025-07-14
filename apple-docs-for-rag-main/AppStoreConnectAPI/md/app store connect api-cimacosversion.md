

- App Store Connect API
-  CiMacOsVersion 

Object

# CiMacOsVersion

The data structure that represents a macOS Versions resource.

App Store Connect API 1.5+

``` source
object CiMacOsVersion
```

## Properties

`attributes`

CiMacOsVersion.Attributes

The attributes that describe the macOS Versions resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a macOS Versions resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

CiMacOsVersion.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `ciMacOsVersions`

## Topics

### Objects

object CiMacOsVersion.Attributes

The attributes that describe a macOS Versions resource.

object CiMacOsVersion.Relationships

The relationships of the macOS Versions resource you included in the request and those on which you can operate.

## See Also

### Objects

object CiMacOsVersionResponse

A response that contains a single macOS Versions resource.

object CiMacOsVersionsResponse

A response that contains a list of macOS Versions resources.

