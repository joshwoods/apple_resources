

- App Store Connect API
- CiXcodeVersion
-  CiXcodeVersion.Attributes 

Object

# CiXcodeVersion.Attributes

The attributes that describe an Xcode Versions resource.

App Store Connect API 1.5+

``` source
object CiXcodeVersion.Attributes
```

## Properties

`name`

`string`

The name of the Xcode version.

`testDestinations`

`[`CiXcodeVersion.Attributes.TestDestinations`]`

A list of the Xcode version’s available test destinations.

`version`

`string`

The Xcode version.

## Topics

### Objects

object CiXcodeVersion.Attributes.TestDestinations

The test destinations available for an Xcode version.

## See Also

### Objects

object CiXcodeVersion.Relationships

The relationships of the Xcode Versions resource you included in the request and those on which you can operate.

