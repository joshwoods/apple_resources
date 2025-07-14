

- Core Image
- CIVector
-  cgAffineTransformValue 

Instance Property

# cgAffineTransformValue

The values in the vector represented as an affine transform.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var cgAffineTransformValue: CGAffineTransform { get }
```

## Discussion

Reading this property creates a CGAffineTransform structure from the first six values in the vector.

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

var cgPointValue: CGPoint

The values in the vector as a Core Graphics point structure.

var cgRectValue: CGRect

The values in the vector as a Core Graphics rectangle structure.

