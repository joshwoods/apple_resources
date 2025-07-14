

- AVFoundation
-  AVCaptureDeviceInput 

Class

# AVCaptureDeviceInput

An object that provides media input from a capture device to a capture session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
class AVCaptureDeviceInput
```

## Mentioned in 

Setting Up a Capture Session

## Overview

This class is a concrete subclass of AVCaptureInput that you use to connect a capture device to a capture session.

## Topics

### Creating an input

init(device: AVCaptureDevice) throws

Creates an input for the specified capture device.

### Configuring video properties

var unifiedAutoExposureDefaultsEnabled: Bool

A Boolean value that indicates whether the input enables unified auto-exposure defaults.

var videoMinFrameDurationOverride: CMTime

A time value that acts as a modifier to a capture device’s active video minimum frame duration.

### Configuring audio properties

func isMultichannelAudioModeSupported(AVCaptureMultichannelAudioMode) -> Bool

A Boolean value that indicates whether the input supports the specified multichannel audio mode.

var multichannelAudioMode: AVCaptureMultichannelAudioMode

The multichannel audio mode to apply when recording audio.

enum AVCaptureMultichannelAudioMode

Constants that indicate the modes of multichannel audio.

### Accessing the Device

var device: AVCaptureDevice

A capture device associated with this input.

func ports(for: AVMediaType?, sourceDeviceType: AVCaptureDevice.DeviceType?, sourceDevicePosition: AVCaptureDevice.Position) -> [AVCaptureInput.Port]

Retrieves a virtual device’s constituent device ports for use in a multi-camera session.

### Instance Properties

var isWindNoiseRemovalEnabled: Bool

var isWindNoiseRemovalSupported: Bool

## Relationships

### Inherits From

- AVCaptureInput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Capture devices

Choosing a Capture Device

Select the front or back camera, or use advanced features like the TrueDepth camera or dual camera.

class AVCaptureDevice

An object that represents a hardware or virtual capture device like a camera or microphone.

class AVContinuityDevice

A class that represents a physical iOS device that’s nearby and can provide access to its cameras and microphones.

class AVExternalStorageDevice

Represents a physical external storage device that stores media assets.

class AVExternalStorageDeviceDiscoverySession

Informs your app when the external storage devices connect to and disconnect from the system.

