

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.SystemPressureState 

Class

# AVCaptureDevice.SystemPressureState

An object that provides information about OS and hardware status affecting capture system performance and availability.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
class SystemPressureState
```

## Overview

The performance and availability of the camera capture system on an iOS device is subject to several external factors, such as power usage and device temperature. If during a capture session the total system pressure reaches excessive levels, the capture system automatically shuts down, causing a session interruption (see wasInterruptedNotification). Under less heavy pressure, the system may automatically reduce capture quality.

Key-value observe the capture device’s systemPressureState property to monitor its state, and take action to reduce the performance impact of your capture session when system pressure increases—for example, by reducing the capture frame rate.

## Topics

### Overall Level

var level: AVCaptureDevice.SystemPressureState.Level

The overall level of performance constraints on the capture system.

struct Level

A structure that defines system pressure state levels.

### Contributing Factors

var factors: AVCaptureDevice.SystemPressureState.Factors

The set of underlying causes for the system pressure level.

struct Factors

A structure that defines the factors affecting capture system performance.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Monitoring System Pressure

var systemPressureState: AVCaptureDevice.SystemPressureState

A value that indicates the capture device’s current system pressure state.

let AVCaptureSessionInterruptionSystemPressureStateKey: String

A key to retrieve a state value that indicates the system pressure level and contributing factors that caused the interruption.

