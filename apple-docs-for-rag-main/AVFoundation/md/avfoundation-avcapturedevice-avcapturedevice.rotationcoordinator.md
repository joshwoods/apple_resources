

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.RotationCoordinator 

Class

# AVCaptureDevice.RotationCoordinator

A class that monitors the physical orientation of a capture device and provides adjustment angles to keep images level, relative to gravity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
class RotationCoordinator
```

## Overview

Correctly rotate the photos and movies your app captures, and optionally, a live camera preview, by applying a coordinator’s videoRotationAngleForHorizonLevelCapture and videoRotationAngleForHorizonLevelPreview properties, respectively. Each rotation coordinator instance updates its properties so that your app can observe them and immediately apply them to the relevant components.

## Topics

### Creating a rotation coordinator

init(device: AVCaptureDevice, previewLayer: CALayer?)

Creates a coordinator that provides separate compensation angles for content your app takes with a capture device, and for your app’s camera preview.

### Compensating for a device’s rotation

var videoRotationAngleForHorizonLevelCapture: CGFloat

An angle the coordinator provides your app to apply to photos or videos it captures with the device so that they’re level relative to gravity.

var videoRotationAngleForHorizonLevelPreview: CGFloat

An angle the coordinator provides your app to apply to the preview layer so that it’s level relative to gravity.

### Inspecting a coordinator’s configuration

var device: AVCaptureDevice?

The capture device the coordinator monitors to track its physical rotation.

var previewLayer: CALayer?

The layer that displays a camera preview the coordinator calculates a video rotation angle for.

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

