

- Core Haptics
-  CHHapticParameterAttributes 

Protocol

# CHHapticParameterAttributes

A protocol for providing default, mininum, and maximum values of a parameter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
protocol CHHapticParameterAttributes : NSObjectProtocol
```

## Topics

### Parameter Attributes

var defaultValue: Float

The default value of the parameter value.

**Required**

var minValue: Float

The minimum value the parameter can take.

**Required**

var maxValue: Float

The maximum value the parameter can take.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Querying System Capabilities

class func capabilitiesForHardware() -> any CHHapticDeviceCapability

Returns a device capability object that describes the device’s haptic support and limitations.

protocol CHHapticDeviceCapability

A protocol that defines haptics and audio capabilities of a device.

func attributes(forDynamicParameter: CHHapticDynamicParameter.ID) throws -> any CHHapticParameterAttributes

Requests the haptic device’s attributes for a dynamic parameter.

**Required**

