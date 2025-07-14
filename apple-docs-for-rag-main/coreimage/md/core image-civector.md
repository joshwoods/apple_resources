

- Core Image
-  CIVector 

Class

# CIVector

A container for coordinate values, direction vectors, matrices, and other non-scalar values, typically used in Core Image for filter parameters.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class CIVector : NSObject
```

## Topics

### Initializing a Vector

init(values: UnsafePointer&lt;CGFloat>, count: Int)

Initializes a vector with the provided values.

init(x: CGFloat)

Initializes the first position of a vector with the provided values.

init(x: CGFloat, y: CGFloat)

Initializes the first two positions of a vector with the provided values.

init(x: CGFloat, y: CGFloat, z: CGFloat)

Initializes the first three positions of a vector with the provided values.

init(x: CGFloat, y: CGFloat, z: CGFloat, w: CGFloat)

Initializes four positions of a vector with the provided values.

init(string: String)

Initializes a vector with values provided in a string representation.

init(cgAffineTransform: CGAffineTransform)

Initializes a vector that is initialized with values provided by a `CGAffineTransform` structure.

init(cgPoint: CGPoint)

Initializes a vector that is initialized with values provided by a `CGPoint` structure.

init(cgRect: CGRect)

Initializes a vector that is initialized with values provided by a `CGRect` structure.

### Getting Values From a Vector

func value(at: Int) -> CGFloat

Returns a value from a specific position in the vector.

var count: Int

The number of items in the vector.

var x: CGFloat

The value located in the first position in the vector.

var y: CGFloat

The value located in the second position in the vector.

var z: CGFloat

The value located in the third position in the vector.

var w: CGFloat

The value located in the fourth position in the vector.

var stringRepresentation: String

The string representation of the vector.

var cgAffineTransformValue: CGAffineTransform

The values in the vector represented as an affine transform.

var cgPointValue: CGPoint

The values in the vector as a Core Graphics point structure.

var cgRectValue: CGRect

The values in the vector as a Core Graphics rectangle structure.

## Relationships

### Inherits From

- NSObject

### Conforms To

- NSCopying
- NSSecureCoding

## See Also

### Filters

class CIFilter

An image processor that produces an image by manipulating one or more input images or by generating new image data.

class CIRAWFilter

A filter subclass that produces an image by manipulating RAW image sensor data from a digital camera or scanner.

class CIColor

The component values defining a color in a specific color space.

