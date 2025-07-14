

- Core Image
- CIVector
-  value(at:) 

Instance Method

# value(at:)

Returns a value from a specific position in the vector.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func value(at index: Int) -> CGFloat
```

## Parameters 

`index`  

The position in the vector of the value that you want to retrieve.

## Return Value

The value retrieved from the vector or `0` if the position is undefined.

## Discussion

The numbering of elements in a vector begins with zero.

## See Also

### Getting Values From a Vector

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

