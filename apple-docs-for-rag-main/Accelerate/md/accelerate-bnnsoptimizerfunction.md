

- Accelerate
-  BNNSOptimizerFunction 

Structure

# BNNSOptimizerFunction

A structure that contains optimizer functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSOptimizerFunction
```

## Topics

### Adam Optimizer Functions

var BNNSOptimizerFunctionAdam: BNNSOptimizerFunction

An optimizer function that updates parameters according to the Adam algorithm.

var BNNSOptimizerFunctionAdamWithClipping: BNNSOptimizerFunction

An optimizer function that updates parameters according to the Adam algorithm and optionally clips the gradient by value or by norm.

var BNNSOptimizerFunctionAdamAMSGrad: BNNSOptimizerFunction

An optimizer function that updates parameters according to the AMSGrad variant of the Adam algorithm.

var BNNSOptimizerFunctionAdamAMSGradWithClipping: BNNSOptimizerFunction

An optimizer function that updates parameters according to the AMSGrad variant of the Adam algorithm and optionally clips the gradient by value or by norm.

### AdamW Optimizer Functions

var BNNSOptimizerFunctionAdamW: BNNSOptimizerFunction

An optimizer function that updates parameters according to the AdamW algorithm.

var BNNSOptimizerFunctionAdamWWithClipping: BNNSOptimizerFunction

An optimizer function that updates parameters according to the AdamW algorithm and optionally clips the gradient by value or by norm.

var BNNSOptimizerFunctionAdamWAMSGrad: BNNSOptimizerFunction

An optimizer function that updates parameters according to the AMSGrad variant of the AdamW algorithm.

var BNNSOptimizerFunctionAdamWAMSGradWithClipping: BNNSOptimizerFunction

An optimizer function that updates parameters according to the AMSGrad variant of the AdamW algorithm and optionally clips the gradient by value or by norm.

### RMSProp Optimizer Functions

var BNNSOptimizerFunctionRMSProp: BNNSOptimizerFunction

An optimizer function that updates parameters according to the root mean square propagation (RMSProp) algorithm.

var BNNSOptimizerFunctionRMSPropWithClipping: BNNSOptimizerFunction

An optimizer function that updates parameters according to the root mean square propagation (RMSProp) algorithm and optionally clips the gradient by value or by norm.

### SGD Optimizer Functions

var BNNSOptimizerFunctionSGDMomentum: BNNSOptimizerFunction

An optimizer function that updates parameters according to the stochastic gradient descent (SGD) with momentum algorithm.

var BNNSOptimizerFunctionSGDMomentumWithClipping: BNNSOptimizerFunction

An optimizer function that updates parameters according to the stochastic gradient descent (SGD) with momentum algorithm and optionally clips the gradient by value or by norm.

### Raw Values

var rawValue: UInt32

init(UInt32)

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

