

- Core Haptics
- CHHapticEngine
-  capabilitiesForHardware() 

Type Method

# capabilitiesForHardware()

Returns a device capability object that describes the device’s haptic support and limitations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
class func capabilitiesForHardware() -> any CHHapticDeviceCapability
```

## See Also

### Querying System Capabilities

protocol CHHapticDeviceCapability

A protocol that defines haptics and audio capabilities of a device.

protocol CHHapticParameterAttributes

A protocol for providing default, mininum, and maximum values of a parameter.

func attributes(forDynamicParameter: CHHapticDynamicParameter.ID) throws -> any CHHapticParameterAttributes

Requests the haptic device’s attributes for a dynamic parameter.

**Required**

