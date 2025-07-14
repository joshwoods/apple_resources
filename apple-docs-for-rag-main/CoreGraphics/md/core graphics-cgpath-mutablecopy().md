

- Core Graphics
- CGPath
-  mutableCopy() 

Instance Method

# mutableCopy()

Creates a mutable copy of an existing graphics path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func mutableCopy() -> CGMutablePath?
```

## Return Value

A new, mutable, copy of the specified path. You are responsible for releasing this object.

## Discussion

You can modify a mutable graphics path by calling the various path geometry functions, such as CGPathAddArc, CGPathAddLineToPoint, and CGPathMoveToPoint.

## See Also

### Copying a Graphics Path

func mutableCopy(using: UnsafePointer&lt;CGAffineTransform>?) -> CGMutablePath?

Creates a mutable copy of a graphics path transformed by a transformation matrix.

