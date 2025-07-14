

- Core Graphics
- CGPath
-  mutableCopy(using:) 

Instance Method

# mutableCopy(using:)

Creates a mutable copy of a graphics path transformed by a transformation matrix.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func mutableCopy(using transform: UnsafePointer?) -> CGMutablePath?
```

## Parameters 

`transform`  

A pointer to an affine transformation matrix, or `NULL` if no transformation is needed. If specified, Core Graphics applies the transformation to all elements of the new path.

## Return Value

A new, mutable copy of the specified path transformed by the transform parameter. You are responsible for releasing this object.

## See Also

### Copying a Graphics Path

func mutableCopy() -> CGMutablePath?

Creates a mutable copy of an existing graphics path.

