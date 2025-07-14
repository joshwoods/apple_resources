

- Core Motion
-  CMRotationMatrix 

Structure

# CMRotationMatrix

The type of a structure representing a rotation matrix.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
struct CMRotationMatrix
```

## Topics

### Fields

Each field in this structure defines an element of the rotation matrix by its position. For example, m11 is the element in row 1, column 1; m31 is the element in row 3, column 1; m13 is the element in row 1, column 3.

var m11: Double

var m12: Double

var m13: Double

var m21: Double

var m22: Double

var m23: Double

var m31: Double

var m32: Double

var m33: Double

### Initializers

init()

init(m11: Double, m12: Double, m13: Double, m21: Double, m22: Double, m23: Double, m31: Double, m32: Double, m33: Double)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Getting a Mathematical Representation of Attitude as a Rotation Matrix

var rotationMatrix: CMRotationMatrix

Returns a rotation matrix representing the device’s attitude.

