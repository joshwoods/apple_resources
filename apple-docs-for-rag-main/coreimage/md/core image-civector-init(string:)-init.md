

- Core Image
- CIVector
-  init(string:) 

Initializer

# init(string:)

Initializes a vector with values provided in a string representation.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
convenience init(string representation: String)
```

## Parameters 

`representation`  

A string that is in one of the formats returned by the `stringRepresentation` method.

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

init(cgAffineTransform: CGAffineTransform)

Initializes a vector that is initialized with values provided by a `CGAffineTransform` structure.

init(cgPoint: CGPoint)

Initializes a vector that is initialized with values provided by a `CGPoint` structure.

init(cgRect: CGRect)

Initializes a vector that is initialized with values provided by a `CGRect` structure.

### Related Documentation

var stringRepresentation: String

The string representation of the vector.

