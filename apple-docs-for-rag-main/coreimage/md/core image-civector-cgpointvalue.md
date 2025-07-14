

- Core Image
- CIVector
-  cgPointValue 

Instance Property

# cgPointValue

The values in the vector as a Core Graphics point structure.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var cgPointValue: CGPoint { get }
```

## Discussion

Reading this property creates a CGPoint structure from the first two values (x and y) in the vector.

## See Also

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

var cgRectValue: CGRect

The values in the vector as a Core Graphics rectangle structure.

