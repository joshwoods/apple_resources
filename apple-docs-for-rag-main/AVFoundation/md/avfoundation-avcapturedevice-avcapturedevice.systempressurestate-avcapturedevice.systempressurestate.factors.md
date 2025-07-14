

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
-  AVCaptureDevice.SystemPressureState.Factors 

Structure

# AVCaptureDevice.SystemPressureState.Factors

A structure that defines the factors affecting capture system performance.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct Factors
```

## Topics

### System Pressure Factors

static var systemTemperature: AVCaptureDevice.SystemPressureState.Factors

The entire system is under elevated thermal load.

static var peakPower: AVCaptureDevice.SystemPressureState.Factors

The system’s peak power requirements exceed the battery’s current capacity.

static var depthModuleTemperature: AVCaptureDevice.SystemPressureState.Factors

The module capturing depth information is operating at an elevated temperature.

static var cameraTemperature: AVCaptureDevice.SystemPressureState.Factors

The camera module is operating at an elevated temperature.

### Initializers

init(rawValue: UInt)

Creates a system pressure factor from its raw string value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Contributing Factors

var factors: AVCaptureDevice.SystemPressureState.Factors

The set of underlying causes for the system pressure level.

