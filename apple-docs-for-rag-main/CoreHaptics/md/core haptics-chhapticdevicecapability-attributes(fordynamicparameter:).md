

- Core Haptics
- CHHapticDeviceCapability
-  attributes(forDynamicParameter:) 

Instance Method

# attributes(forDynamicParameter:)

Requests the haptic device’s attributes for a dynamic parameter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func attributes(forDynamicParameter inParameter: CHHapticDynamicParameter.ID) throws -> any CHHapticParameterAttributes
```

**Required**

## Parameters 

`inParameter`  

The dynamic parameter ID whose attributes you seek.

## Return Value

The haptic device’s attributes for the given dynamic parameter ID.

## See Also

### Querying System Capabilities

class func capabilitiesForHardware() -> any CHHapticDeviceCapability

Returns a device capability object that describes the device’s haptic support and limitations.

protocol CHHapticDeviceCapability

A protocol that defines haptics and audio capabilities of a device.

protocol CHHapticParameterAttributes

A protocol for providing default, mininum, and maximum values of a parameter.

