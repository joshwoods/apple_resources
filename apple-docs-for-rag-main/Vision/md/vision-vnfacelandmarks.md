

- Vision
-  VNFaceLandmarks 

Class

# VNFaceLandmarks

The abstract superclass for containers of face landmark information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNFaceLandmarks
```

## Overview

This class represents the set of all detectable facial landmarks and regions, exposed as properties.

## Topics

### Determining Accuracy

var confidence: VNConfidence

A confidence estimate for the detected landmarks.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VNFaceLandmarks2D

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

## See Also

### Identifying Landmarks

var landmarks: VNFaceLandmarks2D?

The facial features of the detected face.

class VNFaceLandmarks2D

A collection of facial features that a request detects.

class VNFaceLandmarkRegion2D

2D geometry information for a specific facial feature.

class VNFaceLandmarkRegion

The abstract superclass for information about a specific face landmark.

