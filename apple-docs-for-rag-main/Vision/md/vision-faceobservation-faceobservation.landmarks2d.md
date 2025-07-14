

- Vision
- FaceObservation
-  FaceObservation.Landmarks2D 

Structure

# FaceObservation.Landmarks2D

A collection of facial features that a request detects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct Landmarks2D
```

## Overview

This represents the set of all detectable 2D face landmarks and regions, exposed as properties. The coordinates of the face landmarks are normalized to the dimensions of the face observation’s `FaceObservation/boundingBox`, with the origin at the bounding box’s lower-left corner.

## Topics

### Getting the landmarks

var faceContour: FaceObservation.Landmarks2D.Region

var innerLips: FaceObservation.Landmarks2D.Region

var leftEye: FaceObservation.Landmarks2D.Region

var leftEyebrow: FaceObservation.Landmarks2D.Region

var leftPupil: FaceObservation.Landmarks2D.Region

var medianLine: FaceObservation.Landmarks2D.Region

var nose: FaceObservation.Landmarks2D.Region

var noseCrest: FaceObservation.Landmarks2D.Region

var outerLips: FaceObservation.Landmarks2D.Region

var rightEye: FaceObservation.Landmarks2D.Region

var rightEyebrow: FaceObservation.Landmarks2D.Region

var rightPupil: FaceObservation.Landmarks2D.Region

### Inspecting a landmark

let originatingRequestDescriptor: RequestDescriptor?

### Getting all landmarks

var allPoints: FaceObservation.Landmarks2D.Region

struct Region

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let landmarks: FaceObservation.Landmarks2D?

The facial features of the detected face.

let pitch: Measurement&lt;UnitAngle>

The pitch angle of a face.

let roll: Measurement&lt;UnitAngle>

The roll angle of a face.

let yaw: Measurement&lt;UnitAngle>

The yaw angle of a face.

