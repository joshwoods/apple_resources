

- DockKit
- DockAccessory
-  DockAccessory.Observation 

Structure

# DockAccessory.Observation

An observation of the contents of a single video frame.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Observation
```

## Mentioned in 

Track custom objects in a frame

## Overview

This object represents an observation about a single video frame, including information about the type of subject, the coordinates of the subject, and the angle of the subject’s face. DockKit generates tracking vectors from this frame information. When performing your own tracking, you provide one or more DockAccessory.Observation objects to track(_:cameraInformation:).

## Topics

### Creating an observation

init(identifier: Int, type: DockAccessory.Observation.ObservationType, rect: CGRect, faceYawAngle: Measurement&lt;UnitAngle>?)

Creates a new observation.

### Getting properties

let faceYawAngle: Measurement&lt;UnitAngle>?

The angle of the face in radians.

let rect: CGRect

The coordinates of the subject in the frame.

let type: DockAccessory.Observation.ObservationType

The type of subject in the frame.

let identifier: Int

A unique identifier representing the subject in the frame.

### Defining types

enum ObservationType

The available observation types.

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

struct CameraInformation

A collection of tracking information about the camera currently in use.

enum CameraOrientation

The set of camera orientations used to extract coordinates.

