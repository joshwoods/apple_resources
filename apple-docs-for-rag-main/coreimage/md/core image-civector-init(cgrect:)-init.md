

- Core Image
- CIVector
-  init(cgRect:) 

Initializer

# init(cgRect:)

Initializes a vector that is initialized with values provided by a `CGRect` structure.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
convenience init(cgRect r: CGRect)
```

## Parameters 

`r`  

A rect.

## Discussion

The `CGRect` structure’s X, Y, height and width values are stored in the vector’s X, Y, Z and W properties.

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

init(cgAffineTransform: CGAffineTransform)

Initializes a vector that is initialized with values provided by a `CGAffineTransform` structure.

init(cgPoint: CGPoint)

Initializes a vector that is initialized with values provided by a `CGPoint` structure.

