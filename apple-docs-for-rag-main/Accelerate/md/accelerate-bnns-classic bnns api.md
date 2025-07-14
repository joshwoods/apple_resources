

- Accelerate
- BNNS
-  Classic BNNS API 

API Collection

# Classic BNNS API

## Topics

### N-dimensional array descriptor essentials

struct BNNSLayerData

A structure containing common layer parameters.

Deprecated

enum Shape

Constants that describe the size and data layout of an n-dimensional array descriptor.

struct BNNSDataLayout

Constants that describe the data type of an n-dimensional array.

struct BNNSDataType

BNNS Data Types.

struct BNNSNDArrayDescriptor

A structure that describes the shape, stride, data type, and, optionally, the memory location of an n-dimensional array.

func BNNSDataLayoutGetRank(BNNSDataLayout) -> Int

### General filters

typealias BNNSFilter

An opaque type that represents a filter.

Deprecated

Applying Filters

class Layer

The base class for layer objects that wrap filters and manage deinitialization.

Deprecated

class UnaryLayer

The base class for layers that accept a single input.

Deprecated

class BinaryLayer

The base class for layers that accept two inputs.

Deprecated

struct BNNSFilterParameters

A structure that contains common filter parameters.

func BNNSFilterDestroy(BNNSFilter?)

Destroys the specified filter, releasing all resources allocated for it.

Deprecated

typealias BNNSAlloc

A type-alias for a user-provided memory allocation function.

typealias BNNSFree

A type-alias for a user-provided memory deallocation function.

### Activation layers

func BNNSFilterCreateVectorActivationLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?Deprecated

class ActivationLayer

A layer object that wraps an activation filter and manages its deinitialization.

Deprecated

struct BNNSActivationFunction

Constants that describe activation functions.

struct BNNSActivation

A set of parameters that describe common activation functions.

struct BNNSLayerParametersActivation

A set of parameters that define an activation layer.

Deprecated

func BNNSFilterCreateLayerActivation(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new activation layer.

Deprecated

func BNNSDirectApplyActivationBatch(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?, Int, Int, Int) -> Int32

Applies an activation filter to a set of input objects, writing out the result to a set of output objects.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, axes: [Int], input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies an activation function on the specified axes.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies the specified activation function.

Deprecated

### Arithmetic layers

class UnaryArithmeticLayer

A layer object that wraps a unary arithmetic filter and manages its deinitialization.

Deprecated

class BinaryArithmeticLayer

A layer object that wraps a binary arithmetic filter and manages its deinitialization.

Deprecated

class TernaryArithmeticLayer

A layer object that wraps a ternary arithmetic filter and manages its deinitialization.

Deprecated

struct BNNSDescriptorType

Constants that describe the input and output types of an arithmetic operation.

struct BNNSArithmeticUnary

A structure that contains the input and output of an arithmetic operation with a single input.

Deprecated

struct BNNSArithmeticBinary

A structure that contains the inputs and output of an arithmetic operation with two inputs.

Deprecated

struct BNNSArithmeticTernary

A structure that contains the inputs and output of an arithmetic operation with three inputs.

Deprecated

struct BNNSArithmeticFunction

Constants that define arithmetic operations.

struct BNNSLayerParametersArithmetic

A structure that contains the parameters of an arithmetic layer.

Deprecated

func BNNSFilterCreateLayerArithmetic(UnsafePointer&lt;BNNSLayerParametersArithmetic>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new arithmetic layer.

Deprecated

func BNNSArithmeticFilterApplyBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;Int>, UnsafeMutableRawPointer, Int) -> Int32

Applies an arithmetic filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSArithmeticFilterApplyBackwardBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer?>?, UnsafePointer&lt;Int>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafePointer&lt;Int>, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies an arithmetic filter backward to generate input gradients.

Deprecated

### Compute norm functions

static func computeNorm(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?) throws

Computes the Euclidean norm and writes the result to the output tensor.

Deprecated

static func computeNormBackward(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor) throws

Backpropogates gradients for the compute norm function.

Deprecated

func BNNSComputeNorm(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Computes the specified norm over an entire tensor or the specified axes.

Deprecated

func BNNSComputeNormBackward(UnsafeRawPointer, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafeRawPointer, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Backpropogates gradients for the compute norm function.

Deprecated

struct BNNSNormType

Constants that describe norm types.

### Convolution layers

struct BNNSConvolutionLayerParameters

A structure containing convolution parameters.

Deprecated

func BNNSFilterCreateConvolutionLayer(UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSConvolutionLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a convolution filter, initialized with input, output, layer, and filter parameters.

Deprecated

class ConvolutionLayer

A layer object that wraps a convolution filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersConvolution

A structure that contains the parameters of a convolution layer.

Deprecated

func BNNSFilterCreateLayerConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new convolution layer.

Deprecated

func BNNSFilterCreateLayerTransposedConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new transposed convolution layer.

Deprecated

### Crop-resize layers

class CropResizeLayer

A layer object that wraps a crop-resize filter and manages its deinitialization.

Deprecated

func BNNSCropResize(UnsafePointer&lt;BNNSLayerParametersCropResize>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Extracts and resizes regions of interest of an input tensor.

Deprecated

func BNNSCropResizeBackward(UnsafePointer&lt;BNNSLayerParametersCropResize>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a crop-resize filter backward to generate gradients.

Deprecated

struct BNNSLayerParametersCropResize

A set of parameters that describe a crop-resize operation.

Deprecated

struct BNNSBoxCoordinateMode

Constants that define the convention to specify the four bounding box coordinates for crop-resize operations.

struct BNNSLinearSamplingMode

Constants that specify how a crop-resize layer samples a grid.

### Dropout layers

class DropoutLayer

A layer object that wraps a dropout filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersDropout

A structure that contains the parameters of a dropout layer.

Deprecated

func BNNSFilterCreateLayerDropout(UnsafePointer&lt;BNNSLayerParametersDropout>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new dropout layer.

Deprecated

### Embedding layers

class EmbeddingLayer

A layer object that wraps an embedding filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersEmbedding

A structure that contains the parameters of an embedding layer.

Deprecated

func BNNSFilterCreateLayerEmbedding(UnsafePointer&lt;BNNSLayerParametersEmbedding>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new embedding layer.

Deprecated

### Fully connected layers

struct BNNSFullyConnectedLayerParameters

A structure containing fully connected layer parameters.

Deprecated

func BNNSFilterCreateFullyConnectedLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSFullyConnectedLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a fully connected filter, initialized with input, output, layer, and filter parameters.

Deprecated

class FullyConnectedLayer

A layer object that wraps a fully connected filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersFullyConnected

A structure that contains the parameters of a fully connected layer.

Deprecated

func BNNSFilterCreateLayerFullyConnected(UnsafePointer&lt;BNNSLayerParametersFullyConnected>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new fully connected layer.

Deprecated

### Fused layers

protocol FusableLayerParametersDeprecated

class FusedParametersLayer

A layer object that wraps a fused layer and manages its deinitialization.

Deprecated

class FusedConvolutionNormalizationLayer

A layer object that wraps a fused, convolution normalization layer and manages its deinitialization.

Deprecated

class FusedFullyConnectedNormalizationLayer

A layer object that wraps a fused, fully connected normalization layer and manages its deinitialization.

Deprecated

struct BNNSFilterType

Constants that define the component filters of a fused layer.

func BNNSFilterCreateFusedLayer(Int, UnsafePointer&lt;BNNSFilterType>, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new fused layer.

Deprecated

func BNNSFusedFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyMultiInputBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;Int>, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a multiple-input fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?) -> Int32

Applies a fused filter backward to generate input gradients.

Deprecated

func BNNSFusedFilterApplyBackwardMultiInputBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer?>?, UnsafePointer&lt;Int>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafePointer&lt;Int>, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?) -> Int32

Applies a multiple-input fused filter backward to generate input gradients.

Deprecated

### Gather and scatter operations

Calculating the dominant colors in an image

Find the main colors in an image by implementing k-means clustering using the Accelerate framework.

static func gather(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, filterParameters: BNNSFilterParameters?) throws

Gathers the elements of a tensor along a single axis.

Deprecated

static func gatherND(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Gathers the slices of a tensor.

Deprecated

static func scatter(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, reductionFunction: BNNS.ReductionFunction, filterParameters: BNNSFilterParameters?) throws

Scatters the elements of a tensor along a single axis.

Deprecated

static func scatterND(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, reductionFunction: BNNS.ReductionFunction, filterParameters: BNNSFilterParameters?) throws

Scatters the slices of a tensor.

Deprecated

func BNNSGather(Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Gathers the elements of a tensor along a single axis.

Deprecated

func BNNSGatherND(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Gathers the slices of a tensor.

Deprecated

func BNNSScatter(Int, BNNSReduceFunction, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Scatters the elements of a tensor along a single axis.

Deprecated

func BNNSScatterND(BNNSReduceFunction, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Scatters the slices of a tensor.

Deprecated

### Loss layers

class LossLayer

A layer object that wraps a loss filter and manages its deinitialization.

Deprecated

struct BNNSLossFunction

Constants that describe loss functions.

struct BNNSLossReductionFunction

Constants that describe reduction functions used by a loss layer.

struct BNNSLayerParametersLossBase

A structure that contains the parameters of a loss layer.

Deprecated

struct BNNSLayerParametersLossHuber

A structure that contains the parameters of a Huber loss layer.

Deprecated

struct BNNSLayerParametersLossSigmoidCrossEntropy

A structure that contains the parameters of a sigmoid cross entropy loss layer.

Deprecated

struct BNNSLayerParametersLossSoftmaxCrossEntropy

A structure that contains the parameters of a softmax cross entropy loss layer.

Deprecated

struct BNNSLayerParametersLossYolo

A structure that contains the parameters of a You Only Look Once (YOLO) loss layer.

Deprecated

func BNNSFilterCreateLayerLoss(UnsafeRawPointer, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new loss layer.

Deprecated

func BNNSLossFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafeRawPointer?, Int, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int) -> Int32

Applies a loss filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSLossFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeRawPointer, Int, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies a loss filter backward to generate gradients.

Deprecated

### K-nearest neighbors calculation

struct NearestNeighbors

A structure that calculates k-nearest neighbors.

typealias BNNSNearestNeighbors

A k-nearest neighbors object.

func BNNSCreateNearestNeighbors(UInt32, UInt32, UInt32, BNNSDataType, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSNearestNeighbors?

Returns a new k-nearest neighbors object.

func BNNSNearestNeighborsLoad(BNNSNearestNeighbors?, UInt32, UnsafeRawPointer) -> Int32

Adds new sample data to a k-nearest neighbors object.

func BNNSNearestNeighborsGetInfo(BNNSNearestNeighbors?, Int32, UnsafeMutablePointer&lt;Int32>?, UnsafeMutableRawPointer?) -> Int32

Calculates the sorted indices and Euclidean distances of the k-nearest neighbors to a specified sample data point.

func BNNSDestroyNearestNeighbors(BNNSNearestNeighbors?)

Destroys a k-nearest neighbors object.

### Matrix multiplication

func BNNSDirectApplyBroadcastMatMul(Bool, Bool, Float, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?)

Applies a broadcast matrix multiplication operation directly to two input matrices.

Deprecated

class BroadcastMatrixMultiplyLayer

A layer object that wraps a broadcast matrix multiply filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersBroadcastMatMul

A set of parameters that define a broadcast matrix multiply layer.

Deprecated

func BNNSFilterCreateLayerBroadcastMatMul(UnsafePointer&lt;BNNSLayerParametersBroadcastMatMul>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new broadcast matrix multiply layer.

Deprecated

func BNNSMatMulWorkspaceSize(Bool, Bool, Float, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int

Returns the workspace size that a matrix multiply operation requires.

Deprecated

func BNNSMatMul(Bool, Bool, Float, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutableRawPointer?, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a matrix multiplication operation directly to two input matrices.

Deprecated

static func applyMatrixMultiplication(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, workspace: UnsafeMutableRawBufferPointer?, filterParameters: BNNSFilterParameters?) throws

Performs a matrix multiplication operation directly on two input matrices.

Deprecated

static func matrixMultiplicationWorkspaceSize(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, filterParameters: BNNSFilterParameters?) -> Int?

Returns the workspace size that a matrix multiply operation requires.

Deprecated

### Multihead attention layers

struct BNNSMHAProjectionParameters

A structure that contains multihead attention projection parameters.

struct BNNSLayerParametersMultiheadAttention

A structure that contains the parameters of a multihead attention layer.

Deprecated

func BNNSFilterCreateLayerMultiheadAttention(UnsafePointer&lt;BNNSLayerParametersMultiheadAttention>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new multihead attention layer.

Deprecated

func BNNSApplyMultiheadAttention(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a mutihead attention filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSApplyMultiheadAttentionBackward(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>, Int, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a multihead attention filter backward to generate gradients.

Deprecated

### Normalization layers

class NormalizationLayer

A layer object that wraps a normalization filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersNormalization

A structure that contains the parameters of a normalization layer.

Deprecated

func BNNSFilterCreateLayerNormalization(BNNSFilterType, UnsafePointer&lt;BNNSLayerParametersNormalization>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new normalization layer.

Deprecated

func BNNSNormalizationFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a normalization filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSNormalizationFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?) -> Int32

Applies a normalization filter backward to generate gradients.

Deprecated

### Optimizers

struct AdamOptimizer

An optimizer that uses the Adam optimization algorithm.

Deprecated

struct AdamWOptimizer

An optimizer that uses the AdamW optimization algorithm.

Deprecated

struct RMSPropOptimizer

An optimizer that uses the root mean square propagation (RMSProp) optimization method.

Deprecated

struct SGDMomentumOptimizer

An optimizer that uses the stochastic gradient descent (SGD) with the momentum optimization method.

Deprecated

protocol BNNSOptimizerDeprecated

struct BNNSOptimizerRegularizationFunction

A structure that contains optimizer regularization functions.

struct BNNSOptimizerAdamFields

A structure that contains the fields of an Adam optimizer.

Deprecated

struct BNNSOptimizerAdamWithClippingFields

A structure that contains the fields of an Adam or AdamW optimizer that optionally clips the gradient by value or by norm.

Deprecated

struct BNNSOptimizerRMSPropFields

A structure that contains the fields of a root mean square propagation (RMSProp) optimizer.

Deprecated

struct BNNSOptimizerRMSPropWithClippingFields

A structure that contains the fields of a root mean square propagation (RMSProp) optimizer that optionally clips the gradient by value or by norm.

Deprecated

struct BNNSOptimizerSGDMomentumFields

A structure that contains the fields of a stochastic gradient descent (SGD) with momentum optimizer.

Deprecated

struct BNNSOptimizerSGDMomentumWithClippingFields

A structure that contains the fields of a stochastic gradient descent (SGD) with momentum optimizer that optionally clips the gradient by value or by norm.

Deprecated

struct BNNSOptimizerSGDMomentumVariant

Constants that define SGD momentum variants.

func BNNSOptimizerStep(BNNSOptimizerFunction, UnsafeRawPointer, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafeMutablePointer&lt;UnsafePointer&lt;BNNSNDArrayDescriptor>>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a single optimization step to one or more parameters.

Deprecated

struct BNNSOptimizerFunction

A structure that contains optimizer functions.

### Padding layers

class PaddingLayer

A layer object that wraps a padding filter and manages its deinitialization.

Deprecated

struct BNNSPaddingMode

Constants that define padding modes.

struct BNNSLayerParametersPadding

A structure that contains the parameters of a padding layer.

Deprecated

func BNNSFilterCreateLayerPadding(UnsafePointer&lt;BNNSLayerParametersPadding>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new loss layer.

Deprecated

### Permute layers

class PermuteLayer

A layer object that wraps a permute filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersPermute

A structure that contains the parameters of a permute layer.

Deprecated

func BNNSFilterCreateLayerPermute(UnsafePointer&lt;BNNSLayerParametersPermute>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new permute layer.

Deprecated

func BNNSPermuteFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies a permute filter backward to generate gradients.

Deprecated

### Pooling layers

struct BNNSPoolingLayerParameters

A structure containing pooling layer parameters.

Deprecated

func BNNSFilterCreatePoolingLayer(UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSPoolingLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a pooling filter, initialized with input, output, layer, and filter parameters.

Deprecated

class PoolingLayer

A layer object that wraps a pooling filter and manages its deinitialization.

Deprecated

struct BNNSPoolingFunction

Constants that describe pooling functions.

var BNNSPoolingFunctionAverage: BNNSPoolingFunctionDeprecated

var BNNSPoolingFunctionMax: BNNSPoolingFunctionDeprecated

struct BNNSLayerParametersPooling

A structure that contains the parameters of a pooling layer.

Deprecated

func BNNSFilterCreateLayerPooling(UnsafePointer&lt;BNNSLayerParametersPooling>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new pooling layer.

Deprecated

func BNNSPoolingFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, UnsafeMutablePointer&lt;Int>?, Int) -> Int32

Applies a pooling filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSPoolingFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafePointer&lt;Int>?, Int) -> Int32

Applies a pooling filter backward to generate gradients.

Deprecated

func BNNSPoolingFilterApplyBatchEx(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, BNNSDataType, UnsafeMutableRawPointer?, Int) -> Int32

Applies a pooling filter to a set of input objects with support for multiple data types for indices.

Deprecated

func BNNSPoolingFilterApplyBackwardBatchEx(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, BNNSDataType, UnsafeRawPointer?, Int) -> Int32

Applies a pooling filter backward to generate gradients with support for multiple data types for indices.

Deprecated

### Quantization functions

static func quantize(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int?, scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Quantizes the input tensor and writes the result to the output tensor.

Deprecated

static func dequantize(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int?, scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Dequantizes the input tensor and writes the result to the output tensor.

Deprecated

struct BNNSQuantizerFunction

Constants that describe quantization functions.

struct BNNSLayerParametersQuantization

A structure that contains the parameters of a quantization layer.

Deprecated

func BNNSDirectApplyQuantizer(UnsafePointer&lt;BNNSLayerParametersQuantization>, UnsafePointer&lt;BNNSFilterParameters>?, Int, Int, Int) -> Int32

Applies a quantization layer directly to two input matrices.

Deprecated

### Random number generation

class RandomGenerator

A random number generator.

func BNNSCreateRandomGenerator(BNNSRandomGeneratorMethod, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSRandomGenerator?

Returns a new random number generator using an internally generated random seed.

func BNNSCreateRandomGeneratorWithSeed(BNNSRandomGeneratorMethod, UInt64, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSRandomGenerator?

Returns a new random number generator using the specified seed.

struct BNNSRandomGeneratorMethod

Constants that describe random number generation methods.

typealias BNNSRandomGenerator

A pointer to a random number generator object.

func BNNSRandomFillUniformInt(BNNSRandomGenerator?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int64, Int64) -> Int32

Fills the specified tensor with random integer values from the continuous uniform distribution within a range.

func BNNSRandomFillUniformFloat(BNNSRandomGenerator?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Float, Float) -> Int32

Fills the specified tensor with random floating-point values from the continuous uniform distribution within a range.

func BNNSRandomFillNormalFloat(BNNSRandomGenerator?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Float, Float) -> Int32

Fills the specified tensor with random floating-point values mapped to a normal distribution.

func BNNSRandomFillCategoricalFloat(BNNSRandomGenerator?, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Bool) -> Int32

Fills the specified tensor with random values from the categorical distributions with the given event probabilities.

func BNNSRandomGeneratorStateSize(BNNSRandomGenerator?) -> Int

Returns the state size, in bytes, of a random number generator.

func BNNSRandomGeneratorGetState(BNNSRandomGenerator?, Int, UnsafeMutableRawPointer) -> Int32

Returns the state of a random number generator.

func BNNSRandomGeneratorSetState(BNNSRandomGenerator?, Int, UnsafeMutableRawPointer) -> Int32

Sets the state of a random number generator.

func BNNSDestroyRandomGenerator(BNNSRandomGenerator?)

Destroys a random number generator.

### Recurrent layers

Using Long Short-Term Memory Layers (LSTM)

Add long short-term memory (LSTM) layers to recurrent neural networks to avoid long-term dependency problems.

struct BNNSLSTMDataDescriptor

A structure that contains the input-output, hidden, and cell state n-dimensional array descriptors for a long short-term memory (LSTM) layer.

Deprecated

struct BNNSLSTMGateDescriptor

A structure that describes a long short-term memory (LSTM) gate layer.

Deprecated

struct BNNSLayerFlags

Options that control the behavior of a long short-term memory (LSTM) layer.

struct BNNSLayerParametersLSTM

A structure that contains the parameters of a long short-term memory (LSTM) layer.

Deprecated

func BNNSComputeLSTMTrainingCacheCapacity(UnsafePointer&lt;BNNSLayerParametersLSTM>) -> Int

Returns the minimum bytes capacity of the training cache buffer a long short-term memory (LSTM) layer uses when it’s applied.

Deprecated

func BNNSDirectApplyLSTMBatchTrainingCaching(UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSFilterParameters>?, UnsafeMutableRawPointer?, Int) -> Int32

Applies a long short-term memory (LSTM) layer directly to an input.

Deprecated

func BNNSDirectApplyLSTMBatchBackward(UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSLayerParametersLSTM>, UnsafePointer&lt;BNNSFilterParameters>?, UnsafeRawPointer?, Int) -> Int32

Applies a long short-term memory (LSTM) filter backward to generate gradients.

Deprecated

### Reduction layers

class ReductionLayer

A layer object that wraps a reduction filter and manages its deinitialization.

Deprecated

static func applyReduction(BNNS.ReductionFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Applies the specified reduction function.

struct BNNSReduceFunction

Constants that describe reduction functions.

struct BNNSLayerParametersReduction

A set of parameters that define a reduction layer.

func BNNSFilterCreateLayerReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new reduction layer.

Deprecated

func BNNSDirectApplyReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a reduction operation directly to an input tensor.

### Resize layers

class ResizeLayer

A layer object that wraps a resize filter and manages its deinitialization.

Deprecated

struct BNNSInterpolationMethod

Constants that describe interpolation methods.

struct BNNSLayerParametersResize

A structure that contains the parameters of a resize layer.

Deprecated

func BNNSFilterCreateLayerResize(UnsafePointer&lt;BNNSLayerParametersResize>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new resize layer.

Deprecated

### Sparse layers

func BNNSNDArrayGetDataSize(UnsafePointer&lt;BNNSNDArrayDescriptor>) -> Int

Returns the size, in bytes, that an array descriptor requires.

func BNNSNDArrayFullyConnectedSparsifySparseCOO(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSSparsityParameters>?, Int, UnsafeMutableRawPointer?, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Converts a sparse tensor from the standardized coordinate list (COO) layout to a device-specific sparse layout that BNNS fully connected layers use.

Deprecated

func BNNSNDArrayFullyConnectedSparsifySparseCSR(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSSparsityParameters>?, Int, UnsafeMutableRawPointer?, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Converts a sparse tensor from the standardized compressed sparse row (CSR) layout to a device-specific sparse layout that BNNS fully connected layers use.

Deprecated

static func sparsify(batchSize: Int, inputLayout: BNNS.SparseLayout, inputDenseShape: BNNSNDArrayDescriptor, inputValues: BNNSNDArrayDescriptor, output: inout BNNSNDArrayDescriptor, sparseParameters: BNNS.SparseParameters?, workspace: UnsafeMutableRawBufferPointer?, filterParameters: BNNSFilterParameters?) throws

Converts a sparse tensor from a standardized sparse layout to a device-specific sparse layout that Fully Connected uses.

Deprecated

struct SparseParameters

A data structure that provides a hint to the sparsity function.

Deprecated

enum SparseLayout

Constants that specify standardized sparse layouts that BNNS can convert to opaque.

Deprecated

enum SparsityType

Constants that specify patterns in the sparsity.

Deprecated

var BNNSSparsityTypeUnstructured: BNNSSparsityType

### Tensor comparison layers

static func compare(BNNSNDArrayDescriptor, BNNSNDArrayDescriptor, using: BNNS.RelationalOperator, output: BNNSNDArrayDescriptor) throws

Performs an elementwise comparison of two array descriptors using the specified relational operator.

Deprecated

struct BNNSRelationalOperator

Constants that describe relational operations.

func BNNSCompareTensor(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSRelationalOperator, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>) -> Int32

Returns a tensor of Boolean type by comparing or performing a logical operation between two inputs.

Deprecated

### Tensor contraction layers

struct BNNSLayerParametersTensorContraction

A structure that contains the parameters of a tensor-contraction layer.

Deprecated

func BNNSFilterCreateLayerTensorContraction(UnsafePointer&lt;BNNSLayerParametersTensorContraction>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new tensor-contraction layer.

Deprecated

### Top-k layers

static func applyTopK(k: Int, input: BNNSNDArrayDescriptor, bestValues: BNNSNDArrayDescriptor, bestIndices: BNNSNDArrayDescriptor, axis: Int, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies a top-k filter directly to an input.

static func applyInTopK(k: Int, input: BNNSNDArrayDescriptor, testIndices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies an in-top-k filter directly to an input.

### Top-k layers

func BNNSDirectApplyTopK(Int, Int, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a top-k filter directly to an input.

func BNNSDirectApplyInTopK(Int, Int, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies an in-top-k filter directly to an input.

### Utility functions

static func copy(BNNSNDArrayDescriptor, to: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Copies the contents of an n-dimensional array descriptor to another descriptor of the same shape.

static func transpose(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, firstTransposeAxis: Int, secondTransposeAxis: Int, filterParameters: BNNSFilterParameters?) throws

Transposes a tensor by swapping two of its dimensions.

func BNNSCopy(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Copies the contents of an n-dimensional array descriptor to another of the same shape.

func BNNSTranspose(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Transposes a tensor by swapping two of its dimensions.

func BNNSGetPointer(BNNSFilter?, BNNSPointerSpecifier) -> BNNSNDArrayDescriptor

Returns an n-dimensional array descriptor that contains a reference to a filter-data member.

Deprecated

struct BNNSPointerSpecifier

Constants that specify which pointer the BNNS get filter function returns.

class GramLayer

A layer object that wraps a Gram matrix filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersGram

A set of parameters that define a Gram matrix layer.

Deprecated

func BNNSFilterCreateLayerGram(UnsafePointer&lt;BNNSLayerParametersGram>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new Gram matrix layer.

Deprecated

static func clip(to: ClosedRange&lt;Float>, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Clips the input tensor to a closed range and writes the result to the output tensor.

Deprecated

static func clipByNorm(threshold: Float, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?) throws

Clips the input tensor to a Euclidean norm and writes the result to the output tensor.

Deprecated

static func clipByGlobalNorm(threshold: Float, inputs: [BNNSNDArrayDescriptor], outputs: [BNNSNDArrayDescriptor], globalNorm: Float) throws

Clips the input tensors to a global Euclidean norm and writes the result to the output tensors.

Deprecated

func BNNSClipByValue(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Float, Float) -> Int32

Clips a tensor’s values to the specified minimum and maximum values.

Deprecated

func BNNSClipByNorm(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Float, UInt32) -> Int32

Clips a tensor’s values to a maximum Euclidean norm.

Deprecated

func BNNSClipByGlobalNorm(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafeMutablePointer&lt;UnsafePointer&lt;BNNSNDArrayDescriptor>>, Int, Float, Float) -> Int32

Clips a tensor’s values to a maximum global Euclidean norm.

Deprecated

static func copyBandPart(BNNSNDArrayDescriptor, to: BNNSNDArrayDescriptor, lowerBandCount: Int?, upperBandCount: Int?, filterParameters: BNNSFilterParameters?) throws

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

Deprecated

static func shuffle(BNNS.ShuffleType, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Rearranges elements in a tensor according to shuffle type.

Deprecated

enum ShuffleType

Constants that specify a shuffle type.

Deprecated

static func tile(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Generates an output tensor by tiling an input tensor multiple times.

Deprecated

static func tileBackward(outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Applies a tile filter backward to generate an input gradient.

Deprecated

### Errors

enum Error

func BNNSBandPart(Int32, Int32, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

Deprecated

func BNNSShuffle(BNNSShuffleType, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Rearranges elements in a tensor according to shuffle type.

Deprecated

struct BNNSShuffleType

Constants that specify a shuffle type.

func BNNSTile(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Generates an output tensor by tiling an input tensor multiple times.

Deprecated

func BNNSTileBackward(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a tile filter backward to generate an input gradient.

Deprecated

### Macros

var BNNSDataTypeFloat16: BNNSDataTypeDeprecated

var BNNSDataTypeFloat32: BNNSDataTypeDeprecated

var BNNSDataTypeIndexed8: BNNSDataTypeDeprecated

var BNNSDataTypeInt16: BNNSDataTypeDeprecated

var BNNSDataTypeInt32: BNNSDataTypeDeprecated

var BNNSDataTypeInt8: BNNSDataTypeDeprecated

var BNNSFlagsUseClientPtr: BNNSFlagsDeprecated

