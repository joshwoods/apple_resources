

- Nearby Interaction
- NIDeviceCapability
-  supportsCameraAssistance 

Instance Property

# supportsCameraAssistance

A Boolean value that indicates whether the device can leverage ARKit to improve interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
var supportsCameraAssistance: Bool { get }
```

**Required**

## Mentioned in 

Initiating and maintaining a session

## Discussion

For more on Camera Assistance, see isCameraAssistanceEnabled.

Note

Apple Watch doesn’t support Camera Assistance.

## See Also

### Session features

var supportsPreciseDistanceMeasurement: Bool

A Boolean value that indicates whether the device produces precise distance measurements to nearby objects.

**Required**

var supportsDirectionMeasurement: Bool

A Boolean value that indicates whether the device produces instantaneous direction measurements to nearby objects.

**Required**

var supportsExtendedDistanceMeasurement: Bool

A Boolean value that indicates whether this device supports extended distance measurement.

**Required**

