

- Nearby Interaction
- NIDeviceCapability
-  supportsPreciseDistanceMeasurement 

Instance Property

# supportsPreciseDistanceMeasurement

A Boolean value that indicates whether the device produces precise distance measurements to nearby objects.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
var supportsPreciseDistanceMeasurement: Bool { get }
```

**Required**

## Discussion

If false, then the device doesn’t support Nearby Interaction.

This property is functionally equivalent to the deprecated isSupported.

## See Also

### Session features

var supportsDirectionMeasurement: Bool

A Boolean value that indicates whether the device produces instantaneous direction measurements to nearby objects.

**Required**

var supportsCameraAssistance: Bool

A Boolean value that indicates whether the device can leverage ARKit to improve interaction.

**Required**

var supportsExtendedDistanceMeasurement: Bool

A Boolean value that indicates whether this device supports extended distance measurement.

**Required**

