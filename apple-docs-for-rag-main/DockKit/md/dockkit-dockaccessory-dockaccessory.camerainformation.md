

- DockKit
- DockAccessory
-  DockAccessory.CameraInformation 

Structure

# DockAccessory.CameraInformation

A collection of tracking information about the camera currently in use.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.1+

``` source
struct CameraInformation
```

## Overview

Use this class in conjuction with track(_:cameraInformation:) and track(_:cameraInformation:).

## Topics

### Creating the object

init(captureDevice: AVCaptureDevice.DeviceType, cameraPosition: AVCaptureDevice.Position, orientation: DockAccessory.CameraOrientation, cameraIntrinsics: matrix_float3x3?, referenceDimensions: CGSize?)

Creates an object that describes the camera in use for tracking.

### Getting camera information

let cameraPosition: AVCaptureDevice.Position

The physical position of the capture device.

let cameraIntrinsics: matrix_float3x3?

A matrix that represents the characteristics of the lens.

let captureDevice: AVCaptureDevice.DeviceType

The capture device generating the video.

let orientation: DockAccessory.CameraOrientation

The orientation of the capture device.

let referenceDimensions: CGSize?

The size of the video frame.

## Relationships

### Conforms To

- Sendable

## See Also

### Selecting and tracking

func selectSubject(at: CGPoint) async throws

Selects a subject to track at the supplied coordinates.

func track([AVMetadataObject], cameraInformation: DockAccessory.CameraInformation) async throws

Automatically generate and send tracking vectors to the device.

func track([DockAccessory.Observation], cameraInformation: DockAccessory.CameraInformation) async throws

Automatically generate and send tracking vectors to the device.

struct Observation

An observation of the contents of a single video frame.

enum CameraOrientation

The set of camera orientations used to extract coordinates.

