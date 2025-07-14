

- App Store Connect API
- CiXcodeVersion
- CiXcodeVersion.Attributes
-  CiXcodeVersion.Attributes.TestDestinations 

Object

# CiXcodeVersion.Attributes.TestDestinations

The test destinations available for an Xcode version.

App Store Connect API 1.5+

``` source
object CiXcodeVersion.Attributes.TestDestinations
```

## Properties

`availableRuntimes`

`[`CiXcodeVersion.Attributes.TestDestinations.AvailableRuntimes`]`

A list of runtimes available for the Xcode version.

`deviceTypeIdentifier`

`string`

A string that uniquely identifies the simulated device Xcode Cloud uses for a test action; for example, `com.apple.CoreSimulator.SimDeviceType.iPhone-12`.

`deviceTypeName`

`string`

The display name of the simulated device Xcode Cloud uses for a test action; for example, `iPhone 12`.

`kind`

CiTestDestinationKind

A string that indicates whether a test destination is a simulated device or a Mac.

## Topics

### Objects

object CiXcodeVersion.Attributes.TestDestinations.AvailableRuntimes

The data structure that represents the available runtimes for test destinations of an Xcode Versions resource.

