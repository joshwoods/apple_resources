

- Core ML
-  MLTensor 

Structure

# MLTensor

A multi-dimensional array of numerical or Boolean scalars tailored to ML use cases, containing methods to perform transformations and mathematical operations efficiently using a ML compute device.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MLTensor
```

## Topics

### Operators

static func * (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise multiplication.

static func * (MLTensor, MLTensor) -> MLTensor

Computes element-wise multiplication.

static func * (some MLTensorScalar &amp; Numeric, MLTensor) -> MLTensor

Computes element-wise multiplication.

static func *= (inout MLTensor, MLTensor)

Computes element-wise multiplication.

static func + (some MLTensorScalar &amp; Numeric, MLTensor) -> MLTensor

Computes element-wise addition.

static func + (MLTensor, MLTensor) -> MLTensor

Computes element-wise addition.

static func + (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise addition.

static func += (inout MLTensor, MLTensor)

Computes element-wise addition.

static func - (MLTensor) -> MLTensor

Returns the negation of the tensor.

static func - (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise subtraction.

static func - (some MLTensorScalar &amp; Numeric, MLTensor) -> MLTensor

Computes element-wise subtraction.

static func - (MLTensor, MLTensor) -> MLTensor

Computes element-wise subtraction.

static func -= (inout MLTensor, MLTensor)

Computes element-wise subtraction.

static func .! (MLTensor) -> MLTensor

Computes logical not on the tensor’s elements.

static func .!= (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise inequality between two tensors.

static func .!= (MLTensor, MLTensor) -> MLTensor

Computes element-wise inequality between two tensors.

static func .&amp; (MLTensor, MLTensor) -> MLTensor

Computes element-wise logical AND where both operands are expected contain Boolean scalar elements.

static func .== (MLTensor, MLTensor) -> MLTensor

Computes element-wise equality between two tensors.

static func .== (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise equality between two tensors.

static func .> (MLTensor, MLTensor) -> MLTensor

Computes element-wise greater comparison between two tensors.

static func .> (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise greater comparison between two tensors.

static func .&lt; (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise less comparison between two tensors.

static func .&lt; (MLTensor, MLTensor) -> MLTensor

Computes element-wise less comparison between two tensors.

static func .| (MLTensor, MLTensor) -> MLTensor

Computes element-wise logical OR where both operands are expected contain Boolean scalar elements.

static func .^ (MLTensor, MLTensor) -> MLTensor

Computes element-wise logical XOR where both operands are expected contain Boolean scalar elements.

static func .&lt;= (MLTensor, MLTensor) -> MLTensor

Computes element-wise less than or equal to comparison between two tensors.

static func .>= (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise greater than or equal to comparison between two tensors.

static func .&lt;= (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise less than or equal to comparison between two tensors.

static func .>= (MLTensor, MLTensor) -> MLTensor

Computes element-wise greater than or equal to comparison between two tensors.

static func / (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise division.

static func % (MLTensor, MLTensor) -> MLTensor

Computes element-wise remainder of division.

static func % (some MLTensorScalar &amp; Numeric, MLTensor) -> MLTensor

Computes element-wise remainder of division.

static func / (MLTensor, MLTensor) -> MLTensor

Computes element-wise division.

static func % (MLTensor, some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise remainder of division.

static func / (some MLTensorScalar &amp; Numeric, MLTensor) -> MLTensor

Computes element-wise division.

static func %= (inout MLTensor, MLTensor)

Computes element-wise remainder of division.

static func /= (inout MLTensor, MLTensor)

Computes element-wise multiplication.

### Initializers

init&lt;ShapedArray>(ShapedArray)

Creates a tensor from a ML shaped array.

init(some Collection&lt;Float>)

Creates a one-dimensional tensor from scalars.

init(some Collection&lt;Int32>)

Creates a one-dimensional tensor from scalars.

init(some Collection&lt;MLTensor>, alongAxis: Int)

Creates a tensor by stacking the given tensors along the specified axis.

init&lt;Scalar>(Scalar, scalarType: Scalar.Type)

Creates a zero-dimensional tensor from a scalar value.

init&lt;Scalar>(some Collection, scalarType: Scalar.Type)

Creates a one-dimensional tensor from scalars.

init(bytesNoCopy: UnsafeRawBufferPointer, shape: [Int], scalarType: any MLTensorScalar.Type, deallocator: Data.Deallocator)

Creates a tensor with memory content without copying the bytes.

init(concatenating: some Collection&lt;MLTensor>, alongAxis: Int)

Concatenates `tensors` along the `axis` dimension.

init(linearSpaceFrom: Float, through: Float, count: Int)

Creates a one-dimensional tensor representing a sequence from a starting value, up to and including an end value, spaced evenly to generate the number of values specified.

init&lt;Scalar>(linearSpaceFrom: Scalar, through: Scalar, count: Int, scalarType: Scalar.Type)

Creates a one-dimensional tensor representing a sequence from a starting value, up to and including an end value, spaced evenly to generate the number of values specified.

init&lt;Scalar>(ones: [Int], scalarType: Scalar.Type)

Creates a tensor with all scalars set to ones.

init&lt;Scalar>(ones: [Int], scalarType: Scalar.Type)

Creates a tensor with all scalars set to one.

init&lt;Scalar>(randomNormal: [Int], mean: Scalar, standardDeviation: Scalar, seed: UInt64?, scalarType: Scalar.Type)

Creates a tensor with the specified shape, randomly sampling scalar values from a normal distribution.

init&lt;Scalar>(randomUniform: [Int], in: ClosedRange&lt;Scalar>, seed: UInt64?, scalarType: Scalar.Type)

Creates a tensor with the specified shape, randomly sampling scalar values from a uniform distribution in `bounds`.

init&lt;Scalar>(randomUniform: [Int], in: Range&lt;Scalar>, seed: UInt64?, scalarType: Scalar.Type)

Creates a tensor with the specified shape, randomly sampling scalar values from a uniform distribution in `bounds`.

init(rangeFrom: Float, to: Float, by: Float.Stride)

Creates a one-dimensional tensor representing a sequence from a starting value to, but not including, an end value, stepping by the specified amount.

init&lt;Scalar>(rangeFrom: Scalar, to: Scalar, by: Scalar.Stride, scalarType: Scalar.Type)

Creates a one-dimensional tensor representing a sequence from a starting value to, but not including, an end value, stepping by the specified amount.

init(repeating: Float, shape: [Int])

Creates a tensor with the specified shape and a single, repeated scalar value.

init&lt;Scalar>(repeating: Scalar, shape: [Int], scalarType: Scalar.Type)

Creates a tensor with the specified shape and a single, repeated scalar value.

init(shape: [Int], data: Data, scalarType: any MLTensorScalar.Type)

Creates a tensor by copying the given block of data.

init(shape: [Int], scalars: some Collection&lt;Float>)

Creates a tensor with the specified shape and contiguous scalars in first-major order.

init&lt;Scalar>(shape: [Int], scalars: some Collection, scalarType: Scalar.Type)

Creates a tensor with the specified shape and contiguous scalars in row-major order.

init(stacking: some Collection&lt;MLTensor>, alongAxis: Int)

Stacks the given tensors along the `axis` dimension into a new tensor with rank one higher than the current tensor and each tensor.

init(unsafeUninitializedShape: [Int], scalarType: any MLTensorScalar.Type, initializingWith: (UnsafeMutableRawBufferPointer) throws -> Void) rethrows

Creates a tensor with the specified shape, then calls the given closure with a buffer covering the tensor’s uninitialized memory.

init&lt;Scalar>(zeros: [Int], scalarType: Scalar.Type)

Creates a tensor with all scalars set to zero.

init&lt;Scalar>(zeros: [Int], scalarType: Scalar.Type)

Creates a tensor with all scalars set to zero.

### Instance Properties

var isScalar: Bool

A Boolean value indicating whether the tensor is a scalar (when the `rank` is equal to `0`) or not.

var rank: Int

The number of dimensions of the tensor.

var scalarCount: Int

The number of scalar elements in the tensor.

var scalarType: any MLTensorScalar.Type

The type of scalars in the tensor.

var shape: [Int]

The shape of the tensor.

### Instance Methods

func abs() -> MLTensor

Computes the absolute of the tensor’s elements.

func acos() -> MLTensor

Computes the inverse cosine of the tensor’s elements.

func acosh() -> MLTensor

Computes the inverse hyperbolic cosine of the tensor’s elements.

func all(alongAxes: Int..., keepRank: Bool) -> MLTensor

Computes logical AND on elements across the specified axes of a tensor where the scalar type of the tensor is expected to be Boolean.

func all(alongAxes: [Int], keepRank: Bool) -> MLTensor

Computes logical AND on elements across the specified axes of a tensor where the scalar type of the tensor is expected to be Boolean.

func all(keepRank: Bool) -> MLTensor

Computes logical AND on elements across all axes of a tensor where the scalar type of the tensor is expected to be Boolean.

func any(alongAxes: Int..., keepRank: Bool) -> MLTensor

Computes logical OR on elements across the specified axes of a tensor where the scalar type of the tensor is expected to be Boolean.

func any(alongAxes: [Int], keepRank: Bool) -> MLTensor

Computes logical OR on elements across the specified axes of a tensor where the scalar type of the tensor is expected to be Boolean.

func any(keepRank: Bool) -> MLTensor

Computes logical OR on elements across all dimensions of a tensor where the scalar type of the tensor is expected to be Boolean.

func argmax() -> MLTensor

Returns the index of the maximum value of the flattened scalars.

func argmax(alongAxis: Int, keepRank: Bool) -> MLTensor

Returns the indices of the maximum values along the specified axis.

func argmin() -> MLTensor

Returns the index of the minimum value of the flattened scalars.

func argmin(alongAxis: Int, keepRank: Bool) -> MLTensor

Returns the indices of the minimum values along the specified axis.

func argsort(alongAxis: Int, descendingOrder: Bool) -> MLTensor

Returns the indices (or arguments) of a tensor that give its sorted order along the specified axis.

func asin() -> MLTensor

Computes the inverse sine of the tensor’s elements.

func asinh() -> MLTensor

Computes the inverse hyperbolic sine of the tensor’s elements.

func atan() -> MLTensor

Computes the inverse tangent of the tensor’s elements.

func atanh() -> MLTensor

Computes the inverse hyperbolic tangent of the tensor’s elements.

func bandPart(lowerBandCount: Int, upperBandCount: Int) -> MLTensor

Returns a new tensor with the same shape where everything outside a central band in each innermost matrix is set to zero.

func cast(like: MLTensor) -> MLTensor

Casts the elements of the tensor to the scalar type of the given array.

func cast&lt;Scalar>(to: Scalar.Type) -> MLTensor

Casts the elements of the tensor to the given scalar type.

func ceil() -> MLTensor

Computes the ceiling of the tensor’s elements.

func clamped(to: PartialRangeFrom&lt;Float>) -> MLTensor

Clamps all elements to the given lower bound, inclusively.

func clamped(to: PartialRangeThrough&lt;Float>) -> MLTensor

Clamps all elements to the given upper bound, inclusively.

func clamped(to: ClosedRange&lt;Float>) -> MLTensor

Clamps all elements to the given lower and upper bounds, inclusively.

func concatenated(with: MLTensor, alongAxis: Int) -> MLTensor

Returns a concatenated tensor along the specified axis.

func cos() -> MLTensor

Computes the cosine of the tensor’s elements.

func cosh() -> MLTensor

Computes the hyperbolic cosine of the tensor’s elements.

func cumulativeProduct(alongAxis: Int) -> MLTensor

Computes the cumulative product along the specified axis.

func cumulativeSum(alongAxis: Int) -> MLTensor

Computes the cumulative sum along the specified axis.

func exp() -> MLTensor

Computes the natural exponent of the tensor’s elements.

func exp2() -> MLTensor

Computes the exponent with base two of the tensor’s elements.

func expandingShape(at: Int...) -> MLTensor

Returns a shape-expanded tensor with a dimension of 1 inserted at the specified shape indices.

func expandingShape(at: [Int]) -> MLTensor

Returns a shape-expanded tensor with a dimension of 1 inserted at the specified shape indices.

func flattened() -> MLTensor

Reshape to a one-dimensional tensor.

func floor() -> MLTensor

Computes the floor of the tensor’s elements.

func gathering(atIndices: MLTensor) -> MLTensor

Returns a tensor by gathering slices at the specified indices.

func gathering(atIndices: MLTensor, alongAxis: Int) -> MLTensor

Returns a tensor by gathering slices along the given axis at the specified indices.

func log() -> MLTensor

Computes the natural logarithm of the tensor’s elements.

func matmul(MLTensor) -> MLTensor

Multiplies two tensors together using matrix multiplication.

func max(alongAxes: [Int], keepRank: Bool) -> MLTensor

Returns the maximum values along the specified axes.

func max(alongAxes: Int..., keepRank: Bool) -> MLTensor

Returns the maximum values along the specified axes.

func max(keepRank: Bool) -> MLTensor

Returns the maximum value in the array.

func mean(alongAxes: [Int], keepRank: Bool) -> MLTensor

Returns the mean along the specified axes.

func mean(alongAxes: Int..., keepRank: Bool) -> MLTensor

Returns the mean along the specified axes.

func mean(keepRank: Bool) -> MLTensor

Returns the mean along all axes.

func min(alongAxes: Int..., keepRank: Bool) -> MLTensor

Returns the minimum values along the specified axes.

func min(alongAxes: [Int], keepRank: Bool) -> MLTensor

Returns the minimum values along the specified axes.

func min(keepRank: Bool) -> MLTensor

Returns the minimum value in the array.

func padded(forSizes: [(before: Int, after: Int)], mode: MLTensor.PaddingMode) -> MLTensor

Returns a padded tensor according to the specified padding sizes and mode.

func padded(forSizes: [(before: Int, after: Int)], with: Float) -> MLTensor

Returns a tensor padded with the given constant according to the specified padding sizes.

func pow(some MLTensorScalar &amp; Numeric) -> MLTensor

Computes element-wise power of each element with `exponent`.

func pow(MLTensor) -> MLTensor

Computes element-wise power of each element with `exponent`.

func product(alongAxes: Int..., keepRank: Bool) -> MLTensor

Returns the product along the specified axes.

func product(alongAxes: [Int], keepRank: Bool) -> MLTensor

Returns the product along the specified axes.

func product(keepRank: Bool) -> MLTensor

Returns the product along all axes.

func reciprocal() -> MLTensor

Computes the reciprocal of the tensor’s elements.

func replacing(atIndices: MLTensor, with: some MLTensorScalar, alongAxis: Int) -> MLTensor

Replaces slices along the specified indices with the given replacement values.

func replacing(with: MLTensor, atIndices: MLTensor, alongAxis: Int) -> MLTensor

Replaces slices along the specified indices with the given replacement values.

func replacing(with: MLTensor, where: MLTensor) -> MLTensor

Returns a new tensor replacing values from `other` with the corresponding element in `self` where the associated element in `mask` is `true`.

func replacing(with: some MLTensorScalar, where: MLTensor) -> MLTensor

Returns a new tensor replacing the value of `other` with the corresponding element in `self` where the associated element in `mask` is `true`.

func reshaped(to: [Int]) -> MLTensor

Reshape to the specified shape.

func resized(to: (newHeight: Int, newWidth: Int), method: MLTensor.ResizeMethod) -> MLTensor

Resize the tensor’s spatial dimensions to size using the specified method.

func reversed(alongAxes: Int...) -> MLTensor

Returns a new tensor with the specified dimensions reversed.

func reversed(alongAxes: [Int]) -> MLTensor

Returns a new tensor with the specified dimensions reversed.

func round() -> MLTensor

Rounds the tensor’s elements.

func rsqrt() -> MLTensor

Computes reverse square root of the tensor’s elements.

func shapedArray&lt;Scalar>(of: Scalar.Type) async -> MLShapedArray&lt;Scalar>

Returns a materialized representation of the tensor.

func sign() -> MLTensor

Returns the sign of the tensor’s elements.

func sin() -> MLTensor

Computes sine of the tensor’s elements.

func sinh() -> MLTensor

Computes hyperbolic sine of the tensor’s elements.

func softmax(alongAxis: Int) -> MLTensor

Computes the softmax of the specified tensor along the specified axis.

func split(count: Int, alongAxis: Int) -> [MLTensor]

Splits a tensor into multiple tensors. The tensor is split along dimension `axis` into `count` smaller tensors.

func split(sizes: [Int], alongAxis: Int) -> [MLTensor]

Splits a tensor into multiple tensors. The tensor is split into `sizes.shape[0]` parts.

func squareRoot() -> MLTensor

Computes square root of the tensor’s elements.

func squared() -> MLTensor

Computes square of the tensor’s elements.

func squeezingShape() -> MLTensor

Removes all dimensions of size 1 from the shape of the tensor.

func squeezingShape(at: Int...) -> MLTensor

Removes the specified dimensions of size 1 from the shape of the tensor.

func squeezingShape(at: [Int]) -> MLTensor

Removes the specified dimensions of size 1 from the shape of the tensor.

func sum(alongAxes: Int..., keepRank: Bool) -> MLTensor

Returns the sum along the specified axes.

func sum(alongAxes: [Int], keepRank: Bool) -> MLTensor

Returns the sum along the specified axes.

func sum(keepRank: Bool) -> MLTensor

Returns the sum along all axes.

func tan() -> MLTensor

Computes tangent of the tensor’s elements.

func tanh() -> MLTensor

Computes hyperbolic tangent of the tensor’s elements.

func tiled(multiples: [Int]) -> MLTensor

Returns a tensor by replicating its elements multiple times.

func topK(Int) -> (values: MLTensor, indices: MLTensor)

Returns the *k* largest values along the last axis of the tensor.

func transposed() -> MLTensor

Permutes the tensor with dimensions permuted in reverse order.

func transposed(permutation: [Int]) -> MLTensor

Permutes the dimensions of the tensor in the specified order.

func transposed(permutation: Int...) -> MLTensor

Permutes the dimensions of the tensor in the specified order.

func unstacked(alongAxis: Int) -> [MLTensor]

Unpacks the given dimension of a rank-`R` tensor into multiple rank-`(R-1)` tensors.

### Subscripts

subscript((any MLTensorRangeExpression)?...) -> MLTensor

subscript((UnboundedRange_) -> (), (any MLTensorRangeExpression)?...) -> MLTensor

subscript((any MLTensorRangeExpression)?, (UnboundedRange_) -> (), (any MLTensorRangeExpression)?...) -> MLTensor

subscript((any MLTensorRangeExpression)?, (any MLTensorRangeExpression)?, (UnboundedRange_) -> (), (any MLTensorRangeExpression)?...) -> MLTensor

subscript((any MLTensorRangeExpression)?, (any MLTensorRangeExpression)?, (any MLTensorRangeExpression)?, (UnboundedRange_) -> (), (any MLTensorRangeExpression)?...) -> MLTensor

### Enumerations

enum PaddingMode

A mode that dictates how a tensor is padded.

enum ResizeMethod

A resize algorithm.

### Default Implementations

CustomReflectable Implementations

## Relationships

### Conforms To

- Copyable
- CustomReflectable
- CustomStringConvertible
- ExpressibleByArrayLiteral
- ExpressibleByBooleanLiteral
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- Sendable

## See Also

### Model tensor

protocol MLTensorScalar

A type that represents the tensor scalar types supported by the framework. Don’t use this type directly.

protocol MLTensorRangeExpression

A type that can be used to slice a dimension of a tensor. Don’t use this type directly.

func pointwiseMin(MLTensor, MLTensor) -> MLTensor

Computes the element-wise minimum of two tensors.

func pointwiseMax(MLTensor, MLTensor) -> MLTensor

Computes the element-wise maximum of two tensors.

