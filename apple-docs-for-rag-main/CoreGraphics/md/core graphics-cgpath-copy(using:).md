

- Core Graphics
- CGPath
-  copy(using:) 

Instance Method

# copy(using:)

Creates an immutable copy of a graphics path transformed by a transformation matrix.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func copy(using transform: UnsafePointer?) -> CGPath?
```

## Parameters 

`transform`  

A pointer to an affine transformation matrix, or `NULL` if no transformation is needed. If specified, Core Graphics applies the transformation to all elements of the new path.

## Return Value

A new, immutable copy of the path. You are responsible for releasing this object.

## See Also

### Copying a Graphics Path

func copy() -> CGPath?

Creates an immutable copy of a graphics path.

func copy(dashingWithPhase: CGFloat, lengths: [CGFloat], transform: CGAffineTransform) -> CGPath

Returns a new path equivalent to the results of drawing the path with a dashed stroke.

func copy(strokingWithWidth: CGFloat, lineCap: CGLineCap, lineJoin: CGLineJoin, miterLimit: CGFloat, transform: CGAffineTransform) -> CGPath

Returns a new path equivalent to the results of drawing the path with a solid stroke.

func mutableCopy() -> CGMutablePath?

Creates a mutable copy of an existing graphics path.

func mutableCopy(using: UnsafePointer&lt;CGAffineTransform>?) -> CGMutablePath?

Creates a mutable copy of a graphics path transformed by a transformation matrix.

