

- Core Graphics
- CGPath
-  copy(strokingWithWidth:lineCap:lineJoin:miterLimit:transform:) 

Instance Method

# copy(strokingWithWidth:lineCap:lineJoin:miterLimit:transform:)

Returns a new path equivalent to the results of drawing the path with a solid stroke.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func copy(
    strokingWithWidth lineWidth: CGFloat,
    lineCap: CGLineCap,
    lineJoin: CGLineJoin,
    miterLimit: CGFloat,
    transform: CGAffineTransform = .identity
) -> CGPath
```

## Parameters 

`lineWidth`  

The line width to use, in user space units. The value must be greater than `0`.

`lineCap`  

The line cap style to render. (For equivalent CGContext drawing methods, the default style is CGLineCap.butt.)

`lineJoin`  

The line join style to render. (For equivalent CGContext drawing methods, the default style is CGLineJoin.miter.)

`miterLimit`  

A value that limits how sharp individual corners in the path can be when using the CGLineJoin.miter line join style. When the ratio of a the length required for a mitered corner to the line width exceeds this value, that corner uses the CGLineJoin.bevel style instead.

`transform`  

An affine transform to apply to the path before dashing. Defaults to the CGAffineTransformIdentity transform if not specified.

## Return Value

A new path.

## Discussion

The new path is created so that filling the new path draws the same pixels as stroking the original path with the specified line style.

## See Also

### Copying a Graphics Path

func copy() -> CGPath?

Creates an immutable copy of a graphics path.

func copy(using: UnsafePointer&lt;CGAffineTransform>?) -> CGPath?

Creates an immutable copy of a graphics path transformed by a transformation matrix.

func copy(dashingWithPhase: CGFloat, lengths: [CGFloat], transform: CGAffineTransform) -> CGPath

Returns a new path equivalent to the results of drawing the path with a dashed stroke.

func mutableCopy() -> CGMutablePath?

Creates a mutable copy of an existing graphics path.

func mutableCopy(using: UnsafePointer&lt;CGAffineTransform>?) -> CGMutablePath?

Creates a mutable copy of a graphics path transformed by a transformation matrix.

