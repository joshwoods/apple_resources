

- Core Image
- CIVector
-  init(cgAffineTransform:) 

Initializer

# init(cgAffineTransform:)

Initializes a vector that is initialized with values provided by a `CGAffineTransform` structure.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
convenience init(cgAffineTransform r: CGAffineTransform)
```

## Parameters 

`r`  

A transform.

## Discussion

The six values that comprise the affine transform fill the first six positions of the resulting `CIVector` object.

## See Also

### Initializing a Vector

init(values: UnsafePointer&lt;CGFloat>, count: Int)

Initializes a vector with the provided values.

init(x: CGFloat)

Initializes the first position of a vector with the provided values.

init(x: CGFloat, y: CGFloat)

Initializes the first two positions of a vector with the provided values.

init(x: CGFloat, y: CGFloat, z: CGFloat)

Initializes the first three positions of a vector with the provided values.

init(x: CGFloat, y: CGFloat, z: CGFloat, w: CGFloat)

Initializes four positions of a vector with the provided values.

init(string: String)

Initializes a vector with values provided in a string representation.

init(cgPoint: CGPoint)

Initializes a vector that is initialized with values provided by a `CGPoint` structure.

init(cgRect: CGRect)

Initializes a vector that is initialized with values provided by a `CGRect` structure.

