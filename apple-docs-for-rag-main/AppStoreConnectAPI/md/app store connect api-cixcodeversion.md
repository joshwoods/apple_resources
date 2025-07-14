

- App Store Connect API
-  CiXcodeVersion 

Object

# CiXcodeVersion

The data structure that represents an Xcode Versions resource.

App Store Connect API 1.5+

``` source
object CiXcodeVersion
```

## Properties

`attributes`

CiXcodeVersion.Attributes

The attributes that describe the Xcode Versions resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies an Xcode Versions resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

CiXcodeVersion.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `ciXcodeVersions`

## Topics

### Objects

object CiXcodeVersion.Attributes

The attributes that describe an Xcode Versions resource.

object CiXcodeVersion.Relationships

The relationships of the Xcode Versions resource you included in the request and those on which you can operate.

## See Also

### Objects

object CiXcodeVersionResponse

A response that contains a single Xcode Versions resource.

object CiXcodeVersionsResponse

A response that contains a list of Xcode Versions resources.

