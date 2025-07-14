

- Vision
-  VNPoint 

Class

# VNPoint

An immutable object that represents a single 2D point in an image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNPoint
```

## Topics

### Creating a Point

init(x: Double, y: Double)

Creates a point object with the specified coordinates.

convenience init(location: CGPoint)

Creates a point object from the specified Core Graphics point.

class func apply(VNVector, to: VNPoint) -> VNPoint

Creates a point object that’s shifted by the X and Y offsets of the specified vector.

class var zero: VNPoint

A point object that represents the origin.

### Inspecting a Point

var x: Double

The x-coordinate.

var y: Double

The y-coordinate.

var location: CGPoint

The Core Graphics point for this point.

### Calculating Distance

func distance(VNPoint) -> Double

Returns the distance to another point.

class func distance(VNPoint, VNPoint) -> Double

Calculates the distance between two points.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- VNDetectedPoint

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

## See Also

### Body and hand pose detection

Detecting Human Body Poses in Images

Add the capability to detect human body poses to your app using the Vision framework.

Detecting Hand Poses with Vision

Create a virtual drawing app by using Vision’s capability to detect hand poses.

class VNDetectHumanBodyPoseRequest

A request that detects a human body pose.

class VNDetectHumanHandPoseRequest

A request that detects a human hand pose.

class VNRecognizedPointsObservation

An observation that provides the points the analysis recognized.

class VNHumanBodyPoseObservation

An observation that provides the body points the analysis recognized.

class VNHumanHandPoseObservation

An observation that provides the hand points the analysis recognized.

class VNDetectedPoint

An object that represents a normalized point in an image, along with a confidence value.

class VNRecognizedPoint

An object that represents a normalized point in an image, along with an identifier label and a confidence value.

struct VNRecognizedPointKey

The data type for all recognized point keys.

struct VNRecognizedPointGroupKey

The data type for all recognized-point group keys.

