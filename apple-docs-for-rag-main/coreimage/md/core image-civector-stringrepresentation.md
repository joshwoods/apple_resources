

- Core Image
- CIVector
-  stringRepresentation 

Instance Property

# stringRepresentation

The string representation of the vector.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var stringRepresentation: String { get }
```

## Discussion

Some example string representations of vectors :

- `@"[1.0 0.5 0.3]"` — a `vec3` vector whose components are `X = 1.0`, `Y = 0.5`, and `Z = 0.3`

- `@"[10.0 23.0]` — a `vec2` vector whose components are `X = 10.0` and `Y = 23.0`

To create a `CIVector` object from a string representation, use the vectorWithString: method.

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

var cgAffineTransformValue: CGAffineTransform

The values in the vector represented as an affine transform.

var cgPointValue: CGPoint

The values in the vector as a Core Graphics point structure.

var cgRectValue: CGRect

The values in the vector as a Core Graphics rectangle structure.

