

- Core Image
- CIVector
-  init(values:count:) 

Initializer

# init(values:count:)

Initializes a vector with the provided values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init(
    values: UnsafePointer,
    count: Int
)
```

## Parameters 

`values`  

The values to initialize the vector with.

`count`  

The number of values specified by the `values` argument.

## See Also

### Initializing a Vector

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

init(cgRect: CGRect)

Initializes a vector that is initialized with values provided by a `CGRect` structure.

