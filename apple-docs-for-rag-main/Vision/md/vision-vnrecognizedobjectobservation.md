

- Vision
-  VNRecognizedObjectObservation 

Class

# VNRecognizedObjectObservation

A detected object observation with an array of classification labels that classify the recognized object.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class VNRecognizedObjectObservation
```

## Overview

The confidence of the classifications sum up to `1.0.` Multiply the classification confidence with the confidence of this observation.

## Topics

### Classifying a Recognized Object

var labels: [VNClassificationObservation]

An array of observations that classify the recognized object.

class VNClassificationObservation

An object that represents classification information that an image-analysis request produces.

## Relationships

### Inherits From

- VNDetectedObjectObservation

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

### Object recognition

Recognizing Objects in Live Capture

Apply Vision algorithms to identify objects in real-time video.

Understanding a Dice Roll with Vision and Object Detection

Detect dice position and values shown in a camera frame, and determine the end of a roll by leveraging a dice detection model.

