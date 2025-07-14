

- ML Compute
-  MLCMatMulDescriptor Deprecated

Class

# MLCMatMulDescriptor

A configuration object you use to create a matrix multiplication layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCMatMulDescriptor
```

## Topics

### Creating Matrix Multiplication Descriptors

convenience init()

Creates a batched matrix multiplication descriptor.

convenience init?(alpha: Float, transposesX: Bool, transposesY: Bool)

Creates a batched matrix multiplication descriptor with the alpha value and transpose options you specify.

### Inspecting Matrix Multiplication Descriptors

var alpha: Float

A scalar value you specify to scale the result in C = alpha x A x B.

var transposesX: Bool

A Boolean that specifies whether you choose to transpose the last two dimensions of x.

var transposesY: Bool

A Boolean that specifies whether you choose to transpose the last two dimensions of y.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating Matrix Multiplication Layers

convenience init?(descriptor: MLCMatMulDescriptor)

Creates a matrix multiplication layer with the specified descriptor you specify.

Deprecated

