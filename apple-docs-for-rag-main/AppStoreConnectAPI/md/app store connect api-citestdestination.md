

- App Store Connect API
-  CiTestDestination 

Object

# CiTestDestination

The test destination of a test action that Xcode Cloud performs.

App Store Connect API 1.5+

``` source
object CiTestDestination
```

## Properties

`deviceTypeIdentifier`

`string`

A string that uniquely identifies the simulated device Xcode Cloud uses for a test action, for example, `com.apple.CoreSimulator.SimDeviceType.iPhone-12`.

`deviceTypeName`

`string`

The display name of the simulated device that Xcode Cloud uses for a test action, for example, iPhone 12.

`kind`

CiTestDestinationKind

A string that indicates whether a test destination is a simulated device or a Mac.

`runtimeIdentifier`

`string`

A string that identifies the simulated environment that Xcode Cloud uses for a test action.

`runtimeName`

`string`

The name of the operating system of the simulated environment that Xcode Cloud uses for a test action.

## See Also

### Objects and Types

type CiTestDestinationKind

The string that represents the kind of a test destination.

