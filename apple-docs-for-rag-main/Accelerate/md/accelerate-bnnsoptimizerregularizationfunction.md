

- Accelerate
-  BNNSOptimizerRegularizationFunction 

Structure

# BNNSOptimizerRegularizationFunction

A structure that contains optimizer regularization functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSOptimizerRegularizationFunction
```

## Topics

### Regularization Functions

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSOptimizerRegularizationL1: BNNSOptimizerRegularizationFunction

A regularization function that applies L1 regularization.

var BNNSOptimizerRegularizationL2: BNNSOptimizerRegularizationFunction

A regularization function that applies L2 regularization.

var BNNSOptimizerRegularizationNone: BNNSOptimizerRegularizationFunction

A regularization function that adoesn’t apply any regularization.

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

