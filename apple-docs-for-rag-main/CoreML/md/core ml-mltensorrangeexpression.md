

- Core ML
-  MLTensorRangeExpression 

Protocol

# MLTensorRangeExpression

A type that can be used to slice a dimension of a tensor. Don’t use this type directly.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol MLTensorRangeExpression : Sendable
```

## Topics

### Type Properties

static var fillAll: any MLTensorRangeExpression

The same as the ellipsis literal `...` used to indicate unspecified dimensions of the tensor.

static var newAxis: any MLTensorRangeExpression

Expand the tensor at the specified dimension.

static var squeezeAxis: any MLTensorRangeExpression

Squeeze the tensor at the specified dimension.

### Type Methods

static func closedRange(ClosedRange&lt;Int>, stride: Int) -> any MLTensorRangeExpression

Slice the tensor at the specified dimension.

static func index(Int) -> any MLTensorRangeExpression

Slice the tensor at the specified dimension.

static func partialRangeFrom(PartialRangeFrom&lt;Int>, stride: Int) -> any MLTensorRangeExpression

Slice the tensor at the specified dimension.

static func partialRangeUpTo(PartialRangeUpTo&lt;Int>, stride: Int) -> any MLTensorRangeExpression

Slice the tensor at the specified dimension.

static func partialRangeUpTo(PartialRangeThrough&lt;Int>, stride: Int) -> any MLTensorRangeExpression

Slice the tensor at the specified dimension.

static func range(Range&lt;Int>, stride: Int) -> any MLTensorRangeExpression

Slice the tensor at the specified dimension.

## Relationships

### Inherits From

- Sendable

## See Also

### Model tensor

struct MLTensor

A multi-dimensional array of numerical or Boolean scalars tailored to ML use cases, containing methods to perform transformations and mathematical operations efficiently using a ML compute device.

protocol MLTensorScalar

A type that represents the tensor scalar types supported by the framework. Don’t use this type directly.

func pointwiseMin(MLTensor, MLTensor) -> MLTensor

Computes the element-wise minimum of two tensors.

func pointwiseMax(MLTensor, MLTensor) -> MLTensor

Computes the element-wise maximum of two tensors.

