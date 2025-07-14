

- Cinematic
-  CNDetection 

Structure

# CNDetection

A structure that represents a detected subject, face, torso or pet at a particular time.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
struct CNDetection
```

## Overview

Specifies the type, distance bounds, and time of the detection. Detections obtained from the Cinematic script include a unique number that can tracks the detection over time.

Some types of detections also include a unique group number that associates related detections (for example, the face and torso of the same person).

## Topics

### Initializers

init(time: CMTime, detectionType: CNDetectionType, normalizedRect: CGRect, focusDisparity: Float)

Creates a Cinematic detection of a subject.

### Instance Properties

var detectionGroupID: CNDetectionGroupID?

A unique number representing the detection to focus on if this is a group decision.

var detectionID: CNDetectionID?

An unique identifier assigned by the Cinematic script to all detections of the same subject and detection type across time.

var detectionType: CNDetectionType

The type of object detected, such as the face, torso, cat, dog, and so on.

var focusDisparity: Float

The disparity to use in order to focus on the object.

var normalizedRect: CGRect

The rectangle within the image where the object occurs, normalized such that (0.0, 0.0) is the top-left and (1.0, 1.0) is the bottom-right.

var time: CMTime

The first presentation time which the subject should be in focus.

### Type Methods

static func accessibilityLabel(for: CNDetectionType) -> String

A localized accessibility label converting a specific detection type into a broad category such as a person, pet, and so on.

static func disparity(in: CGRect, sourceDisparity: CVPixelBuffer, detectionType: CNDetectionType, priorDisparity: Float?) -> Float

Determines the disparity to use to focus on the object in the rectangle.

## Relationships

### Conforms To

- Sendable

## See Also

### Editing

struct CNDecision

An object that represents a decision to focus on a particular detection, or group of detections, at a particular time.

class CNDetectionTrack

An object representing a series of detections of the same subject over time.

class CNFixedDetectionTrack

An object representing the fixed detection track.

class CNCustomDetectionTrack

An object representing a discrete detection track composed of individual detections.

enum CNDetectionType

The type of object detected, such as face, torso, cat, dog and so on.

