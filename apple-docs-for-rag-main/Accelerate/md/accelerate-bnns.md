

- Accelerate
-  BNNS 

Enumeration

# BNNS

An enumeration that acts as a namespace for Swift overlays to BNNS.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum BNNS
```

## Topics

### Base Classes

class Layer

The base class for layer objects that wrap filters and manage deinitialization.

Deprecated

class UnaryLayer

The base class for layers that accept a single input.

Deprecated

class BinaryLayer

The base class for layers that accept two inputs.

Deprecated

### Classes

class ActivationLayer

A layer object that wraps an activation filter and manages its deinitialization.

Deprecated

class BinaryArithmeticLayer

A layer object that wraps a binary arithmetic filter and manages its deinitialization.

Deprecated

class BroadcastMatrixMultiplyLayer

A layer object that wraps a broadcast matrix multiply filter and manages its deinitialization.

Deprecated

class ConvolutionLayer

A layer object that wraps a convolution filter and manages its deinitialization.

Deprecated

class CropResizeLayer

A layer object that wraps a crop-resize filter and manages its deinitialization.

Deprecated

class DropoutLayer

A layer object that wraps a dropout filter and manages its deinitialization.

Deprecated

class EmbeddingLayer

A layer object that wraps an embedding filter and manages its deinitialization.

Deprecated

class FullyConnectedLayer

A layer object that wraps a fully connected filter and manages its deinitialization.

Deprecated

class FusedConvolutionNormalizationLayer

A layer object that wraps a fused, convolution normalization layer and manages its deinitialization.

Deprecated

class FusedFullyConnectedNormalizationLayer

A layer object that wraps a fused, fully connected normalization layer and manages its deinitialization.

Deprecated

class FusedLayer

The base class for fused convolution-normalization and fully connected-normalization layers.

Deprecated

class FusedParametersLayer

A layer object that wraps a fused layer and manages its deinitialization.

Deprecated

class GramLayer

A layer object that wraps a Gram matrix filter and manages its deinitialization.

Deprecated

class LossLayer

A layer object that wraps a loss filter and manages its deinitialization.

Deprecated

class NormalizationLayer

A layer object that wraps a normalization filter and manages its deinitialization.

Deprecated

class PaddingLayer

A layer object that wraps a padding filter and manages its deinitialization.

Deprecated

class PermuteLayer

A layer object that wraps a permute filter and manages its deinitialization.

Deprecated

class PoolingLayer

A layer object that wraps a pooling filter and manages its deinitialization.

Deprecated

class RandomGenerator

A random number generator.

class RandomGeneratorState

An opaque object that contains the state of a random number generator.

class ReductionLayer

A layer object that wraps a reduction filter and manages its deinitialization.

Deprecated

class ResizeLayer

A layer object that wraps a resize filter and manages its deinitialization.

Deprecated

class TernaryArithmeticLayer

A layer object that wraps a ternary arithmetic filter and manages its deinitialization.

Deprecated

class UnaryArithmeticLayer

A layer object that wraps a unary arithmetic filter and manages its deinitialization.

Deprecated

### Structures

struct AdamOptimizer

An optimizer that uses the Adam optimization algorithm.

Deprecated

struct AdamWOptimizer

An optimizer that uses the AdamW optimization algorithm.

Deprecated

struct FusedBinaryArithmeticParameters

A structure that contains the parameters for a fused binary arithmetic layer.

Deprecated

struct FusedConvolutionParameters

A structure that contains the parameters for a fused convolution layer.

Deprecated

struct FusedDequantizationParameters

A structure that contains the parameters for a fused dequantization layer.

Deprecated

struct FusedFullyConnectedParameters

A structure that contains the parameters for a fused fully connected layer.

Deprecated

struct FusedNormalizationParameters

A structure that contains the parameters for a fused normalization layer.

Deprecated

struct FusedQuantizationParameters

A structure that contains the parameters for a fused quantization layer.

Deprecated

struct FusedTernaryArithmeticParameters

A structure that contains the parameters for a fused ternary arithmetic layer.

Deprecated

struct FusedUnaryArithmeticParameters

A structure that contains the parameters for a fused unary arithmetic layer.

Deprecated

struct NearestNeighbors

A structure that calculates k-nearest neighbors.

struct Norm

Constants that describe norm types.

Deprecated

struct RMSPropOptimizer

An optimizer that uses the root mean square propagation (RMSProp) optimization method.

Deprecated

struct RelationalOperator

Constants that describe relational operations.

Deprecated

struct SGDMomentumOptimizer

An optimizer that uses the stochastic gradient descent (SGD) with the momentum optimization method.

Deprecated

struct SparseParameters

A data structure that provides a hint to the sparsity function.

Deprecated

### Type Methods

static func applyActivation(activation: BNNS.ActivationFunction, axes: [Int], input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies an activation function on the specified axes.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies the specified activation function.

Deprecated

static func applyInTopK(k: Int, input: BNNSNDArrayDescriptor, testIndices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies an in-top-k filter directly to an input.

static func applyMatrixMultiplication(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, workspace: UnsafeMutableRawBufferPointer?, filterParameters: BNNSFilterParameters?) throws

Performs a matrix multiplication operation directly on two input matrices.

Deprecated

static func applyReduction(BNNS.ReductionFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Applies the specified reduction function.

static func applyTopK(k: Int, input: BNNSNDArrayDescriptor, bestValues: BNNSNDArrayDescriptor, bestIndices: BNNSNDArrayDescriptor, axis: Int, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies a top-k filter directly to an input.

static func clip(to: ClosedRange&lt;Float>, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Clips the input tensor to a closed range and writes the result to the output tensor.

Deprecated

static func clipByGlobalNorm(threshold: Float, inputs: [BNNSNDArrayDescriptor], outputs: [BNNSNDArrayDescriptor], globalNorm: Float) throws

Clips the input tensors to a global Euclidean norm and writes the result to the output tensors.

Deprecated

static func clipByNorm(threshold: Float, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?) throws

Clips the input tensor to a Euclidean norm and writes the result to the output tensor.

Deprecated

static func compare(BNNSNDArrayDescriptor, BNNSNDArrayDescriptor, using: BNNS.RelationalOperator, output: BNNSNDArrayDescriptor) throws

Performs an elementwise comparison of two array descriptors using the specified relational operator.

Deprecated

static func computeNorm(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?) throws

Computes the Euclidean norm and writes the result to the output tensor.

Deprecated

static func computeNormBackward(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor) throws

Backpropogates gradients for the compute norm function.

Deprecated

static func copy(BNNSNDArrayDescriptor, to: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Copies the contents of an n-dimensional array descriptor to another descriptor of the same shape.

static func copyBandPart(BNNSNDArrayDescriptor, to: BNNSNDArrayDescriptor, lowerBandCount: Int?, upperBandCount: Int?, filterParameters: BNNSFilterParameters?) throws

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

Deprecated

static func dequantize(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int?, scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Dequantizes the input tensor and writes the result to the output tensor.

Deprecated

static func gather(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, filterParameters: BNNSFilterParameters?) throws

Gathers the elements of a tensor along a single axis.

Deprecated

static func gatherND(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Gathers the slices of a tensor.

Deprecated

static func matrixMultiplicationWorkspaceSize(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, filterParameters: BNNSFilterParameters?) -> Int?

Returns the workspace size that a matrix multiply operation requires.

Deprecated

static func quantize(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int?, scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Quantizes the input tensor and writes the result to the output tensor.

Deprecated

static func scatter(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, filterParameters: BNNSFilterParameters?) throws

static func scatter(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, reductionFunction: BNNS.ReductionFunction, filterParameters: BNNSFilterParameters?) throws

Scatters the elements of a tensor along a single axis.

Deprecated

static func scatterND(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

static func scatterND(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, reductionFunction: BNNS.ReductionFunction, filterParameters: BNNSFilterParameters?) throws

Scatters the slices of a tensor.

Deprecated

static func shuffle(BNNS.ShuffleType, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Rearranges elements in a tensor according to shuffle type.

Deprecated

static func tile(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Generates an output tensor by tiling an input tensor multiple times.

Deprecated

static func tileBackward(outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Applies a tile filter backward to generate an input gradient.

Deprecated

static func transpose(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, firstTransposeAxis: Int, secondTransposeAxis: Int, filterParameters: BNNSFilterParameters?) throws

Transposes a tensor by swapping two of its dimensions.

### Enumerations

enum ActivationFunction

Constants that describe activation functions.

Deprecated

enum ArithmeticBinaryFunction

Constants that describe binary arithmetic functions.

Deprecated

enum ArithmeticTernaryFunction

Constants that describe ternary arithmetic functions.

Deprecated

enum ArithmeticUnaryFunction

Constants that describe unary arithmetic functions.

Deprecated

enum ConvolutionPadding

Constants that describe convolution padding modes.

Deprecated

enum ConvolutionType

Constants that describe convolution types.

Deprecated

enum DataLayout

Constants that describe the data layout of an n-dimensional array descriptor shape.

enum DescriptorType

Constants that describe the input and output types of an arithmetic operation.

Deprecated

enum Error

enum GradientClipping

Constants that describe clipping functions.

enum InterpolationMethod

Constants that specify interpolation methods for resize operations.

Deprecated

enum LearningPhase

Constants that describe the learning phase of a normalization operation.

Deprecated

enum LossFunction

Constants that describe loss functions.

Deprecated

enum LossReduction

An enumeration that describes loss reduction functions.

Deprecated

enum NormalizationType

Constants that describe normalization types.

Deprecated

enum PaddingMode

Constants that define padding modes.

Deprecated

enum PoolingType

Constants that describe pooling types.

Deprecated

enum RandomGeneratorMethod

Constants that describe random number generation methods.

enum ReductionFunction

Constants that describe reduction functions.

enum Shape

Constants that describe the size and data layout of an n-dimensional array descriptor.

enum ShuffleType

Constants that specify a shuffle type.

Deprecated

enum SparseLayout

Constants that specify standardized sparse layouts that BNNS can convert to opaque.

Deprecated

enum SparsityType

Constants that specify patterns in the sparsity.

Deprecated

## See Also

### Enumerations

enum BNNSGraph

An enumeration that acts as a namespace for the Swift overlays to BNNS Graph.

