

- Accelerate
-  BNNSActivation 

Structure

# BNNSActivation

A set of parameters that describe common activation functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSActivation
```

## Topics

### Initializers

init()

Returns a new common activation function parameters structure.

init(function: BNNSActivationFunction, alpha: Float, beta: Float)

Returns a new common activation function parameters structure that uses the specified function, alpha, and beta.

Deprecated

init(function: BNNSActivationFunction, alpha: Float, beta: Float, iscale: Int32, ioffset: Int32, ishift: Int32, iscale_per_channel: UnsafePointer&lt;Int32>?, ioffset_per_channel: UnsafePointer&lt;Int32>?, ishift_per_channel: UnsafePointer&lt;Int32>?)

Returns a new common activation function parameters structure that uses the specified function, alpha, beta, integer scale, offset, and shift.

### Instance Properties

var function: BNNSActivationFunction

The activation function that the layer applies to its output.

var alpha: Float

The parameter for the alpha of the activation function.

var beta: Float

The parameter for the beta of the activation function.

var iscale: Int32

Scale for integer functions.

var ioffset: Int32

Offset for integer functions.

var ishift: Int32

Shift for integer functions.

var iscale_per_channel: UnsafePointer&lt;Int32>?

Scale per channel for integer functions.

var ioffset_per_channel: UnsafePointer&lt;Int32>?

Offset per channel for integer functions.

var ishift_per_channel: UnsafePointer&lt;Int32>?

Shift per channel for integer functions.

### Type Methods

static func integerLinearSaturate(scale: Int32, offset: Int32, shift: Int32) -> BNNSActivation

Returns an activation function that computes an arithmetic shift, preserving sign.

Deprecated

static func integerLinearSaturatePerChannel(scale: UnsafePointer&lt;Int32>, offset: UnsafePointer&lt;Int32>, shift: UnsafePointer&lt;Int32>) -> BNNSActivation

Returns an activation function that computes an arithmetic shift, preserving sign for each channel.

Deprecated

### Type Properties

static var identity: BNNSActivation

Identity activation function.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Activation layers

func BNNSFilterCreateVectorActivationLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?Deprecated

class ActivationLayer

A layer object that wraps an activation filter and manages its deinitialization.

Deprecated

struct BNNSActivationFunction

Constants that describe activation functions.

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

