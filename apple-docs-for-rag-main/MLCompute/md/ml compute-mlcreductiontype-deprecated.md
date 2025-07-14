

- ML Compute
-  MLCReductionType Deprecated

Enumeration

# MLCReductionType

Constants that describe a reduction operation type.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCReductionType
```

## Topics

### Enumeration Cases

case all

A reduction operation that applies to all dimensions.

case any

A reduction operation that applies to any dimension.

case argMax

A reduction operation that applies to the maximum dimension you specify.

case argMin

A reduction operation that applies to the minimum dimension you specify.

case max

A reduction operation that applies to the maximum dimension.

case mean

A reduction operation that applies to the mean of the dimensions.

case min

A reduction operation that applies to the minimum dimension.

case none

A reduction operation that applies no reduction.

case sum

A reduction operation that applies to the sum of the dimensions.

case l1Norm

A reduction operation that applies a lasso regularization penalty.

var debugDescription: String

A textual description of the reduction operation you use for debugging.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Reduction Layers

convenience init?(reductionType: MLCReductionType, dimension: Int)

Creates a reduction layer using the reduction type and dimension you specify.

Deprecated

convenience init?(reductionType: MLCReductionType, dimensions: [Int])

Creates a reduction layer using the reduction type and dimensions you specify.

Deprecated

