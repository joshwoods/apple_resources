

- Nearby Interaction
-  NIDeviceCapability 

Protocol

# NIDeviceCapability

An interface that adds Boolean values that indicate an interaction session feature support.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
protocol NIDeviceCapability
```

## Overview

The NISession class property deviceCapabilities adopts this protocol. At runtime, inspect this property to determine the available features of an interaction session on the person’s device.

In a compatible iPad or iPhone app running in visionOS, the framework reports that all capabilities are unavailable.

## Topics

### Session features

var supportsPreciseDistanceMeasurement: Bool

A Boolean value that indicates whether the device produces precise distance measurements to nearby objects.

**Required**

var supportsDirectionMeasurement: Bool

A Boolean value that indicates whether the device produces instantaneous direction measurements to nearby objects.

**Required**

var supportsCameraAssistance: Bool

A Boolean value that indicates whether the device can leverage ARKit to improve interaction.

**Required**

var supportsExtendedDistanceMeasurement: Bool

A Boolean value that indicates whether this device supports extended distance measurement.

**Required**

## See Also

### Ensuring feature support

class var deviceCapabilities: any NIDeviceCapability

An object that communicates the device’s supported framework features.

