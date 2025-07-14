

- Core Graphics
- CGPath
-  copy(dashingWithPhase:lengths:transform:) 

Instance Method

# copy(dashingWithPhase:lengths:transform:)

Returns a new path equivalent to the results of drawing the path with a dashed stroke.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func copy(
    dashingWithPhase phase: CGFloat,
    lengths: [CGFloat],
    transform: CGAffineTransform = .identity
) -> CGPath
```

## Parameters 

`phase`  

A value that specifies how far into the dash pattern the line starts, in units of the user space. For example, a value of `0` draws a line starting with the beginning of a dash pattern, and a value of `3` means the line is drawn with the dash pattern starting at three units from its beginning.

`lengths`  

An array of values that specify the lengths, in user space coordinates, of the painted and unpainted segments of the dash pattern.

For example, the array `[2,3]` sets a dash pattern that alternates between a 2-unit-long painted segment and a 3-unit-long unpainted segment. The array `[1,3,4,2]` sets the pattern to a 1-unit painted segment, a 3-unit unpainted segment, a 4-unit painted segment, and a 2-unit unpainted segment.Pass an empty array to clear the dash pattern so that all stroke drawing in the context uses solid lines.

`transform`  

An affine transform to apply to the path before dashing. Defaults to the CGAffineTransformIdentity transform if not specified.

## Return Value

A new path.

## Discussion

The new path is created so that filling the new path draws the same pixels as stroking the original path with the specified dash parameters.

## See Also

### Copying a Graphics Path

func copy() -> CGPath?

Creates an immutable copy of a graphics path.

func copy(using: UnsafePointer&lt;CGAffineTransform>?) -> CGPath?

Creates an immutable copy of a graphics path transformed by a transformation matrix.

func copy(strokingWithWidth: CGFloat, lineCap: CGLineCap, lineJoin: CGLineJoin, miterLimit: CGFloat, transform: CGAffineTransform) -> CGPath

Returns a new path equivalent to the results of drawing the path with a solid stroke.

func mutableCopy() -> CGMutablePath?

Creates a mutable copy of an existing graphics path.

func mutableCopy(using: UnsafePointer&lt;CGAffineTransform>?) -> CGMutablePath?

Creates a mutable copy of a graphics path transformed by a transformation matrix.

