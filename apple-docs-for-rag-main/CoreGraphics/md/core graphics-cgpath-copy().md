

- Core Graphics
- CGPath
-  copy() 

Instance Method

# copy()

Creates an immutable copy of a graphics path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func copy() -> CGPath?
```

## Return Value

A new, immutable copy of the specified path. You are responsible for releasing this object.

## See Also

### Copying a Graphics Path

func copy(using: UnsafePointer&lt;CGAffineTransform>?) -> CGPath?

Creates an immutable copy of a graphics path transformed by a transformation matrix.

func copy(dashingWithPhase: CGFloat, lengths: [CGFloat], transform: CGAffineTransform) -> CGPath

Returns a new path equivalent to the results of drawing the path with a dashed stroke.

func copy(strokingWithWidth: CGFloat, lineCap: CGLineCap, lineJoin: CGLineJoin, miterLimit: CGFloat, transform: CGAffineTransform) -> CGPath

Returns a new path equivalent to the results of drawing the path with a solid stroke.

func mutableCopy() -> CGMutablePath?

Creates a mutable copy of an existing graphics path.

func mutableCopy(using: UnsafePointer&lt;CGAffineTransform>?) -> CGMutablePath?

Creates a mutable copy of a graphics path transformed by a transformation matrix.

