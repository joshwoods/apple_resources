

- Core Haptics
-  CHHapticDeviceCapability 

Protocol

# CHHapticDeviceCapability

A protocol that defines haptics and audio capabilities of a device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
protocol CHHapticDeviceCapability
```

## Topics

### Determining Support for Haptics

var supportsAudio: Bool

A Boolean value that indicates whether the device supports audio event playback.

**Required**

var supportsHaptics: Bool

A Boolean value that indicates whether the device supports haptic event playback.

**Required**

### Determining Supported Parameters

func attributes(forDynamicParameter: CHHapticDynamicParameter.ID) throws -> any CHHapticParameterAttributes

Requests the haptic device’s attributes for a dynamic parameter.

**Required**

func attributes(forEventParameter: CHHapticEvent.ParameterID, eventType: CHHapticEvent.EventType) throws -> any CHHapticParameterAttributes

Returns the haptic device’s attributes for an event parameter.

**Required**

## See Also

### Querying System Capabilities

class func capabilitiesForHardware() -> any CHHapticDeviceCapability

Returns a device capability object that describes the device’s haptic support and limitations.

protocol CHHapticParameterAttributes

A protocol for providing default, mininum, and maximum values of a parameter.

func attributes(forDynamicParameter: CHHapticDynamicParameter.ID) throws -> any CHHapticParameterAttributes

Requests the haptic device’s attributes for a dynamic parameter.

**Required**

