

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
-  AVCaptureDevice.SystemPressureState.Level 

Structure

# AVCaptureDevice.SystemPressureState.Level

A structure that defines system pressure state levels.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct Level
```

## Topics

### System Pressure Levels

static let nominal: AVCaptureDevice.SystemPressureState.Level

A level that indicates the system pressure is normal and not under pressure.

static let fair: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is slightly elevated.

static let serious: AVCaptureDevice.SystemPressureState.Level

A level that indicates that system pressure is highly elevated.

static let critical: AVCaptureDevice.SystemPressureState.Level

System pressure is critically elevated.

static let shutdown: AVCaptureDevice.SystemPressureState.Level

System pressure is beyond critical, so the capture system has shut down.

### Initializers

init(rawValue: String)

Creates a system pressure level from its raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Overall Level

var level: AVCaptureDevice.SystemPressureState.Level

The overall level of performance constraints on the capture system.

