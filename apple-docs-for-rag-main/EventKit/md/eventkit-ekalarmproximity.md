

- EventKit
-  EKAlarmProximity 

Enumeration

# EKAlarmProximity

A value indicating whether an alarm is triggered by entering or exiting a region.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKAlarmProximity
```

## Topics

### Constants

case none

The alarm has no proximity trigger.

case enter

The alarm is set to fire when entering a region.

case leave

The alarm is set to fire when leaving a region.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting GeoFence-based Alarms

var proximity: EKAlarmProximity

A value indicating how a location-based alarm is triggered.

var structuredLocation: EKStructuredLocation?

The location to trigger an alarm.

