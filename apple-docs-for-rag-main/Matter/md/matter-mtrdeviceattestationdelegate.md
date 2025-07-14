

- Matter
-  MTRDeviceAttestationDelegate 

Protocol

# MTRDeviceAttestationDelegate

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.1+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol MTRDeviceAttestationDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func deviceAttestation(MTRDeviceController, completedForDevice: UnsafeMutableRawPointer, attestationDeviceInfo: MTRDeviceAttestationDeviceInfo, error: (any Error)?)Deprecated

func deviceAttestation(MTRDeviceController, failedForDevice: UnsafeMutableRawPointer, error: any Error)Deprecated

func deviceAttestationCompleted(for: MTRDeviceController, opaqueDeviceHandle: UnsafeMutableRawPointer, attestationDeviceInfo: MTRDeviceAttestationDeviceInfo, error: (any Error)?)

func deviceAttestationFailed(for: MTRDeviceController, opaqueDeviceHandle: UnsafeMutableRawPointer, error: any Error)

## Relationships

### Inherits From

- NSObjectProtocol

