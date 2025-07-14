

- Accelerate
-  BNNSOptimizer Deprecated

Protocol

# BNNSOptimizer

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
protocol BNNSOptimizer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Instance Properties

var accumulatorCountMultiplier: Int

**Required**

var bnnsOptimizerFunction: BNNSOptimizerFunction

**Required**

### Instance Methods

func step(parameters: [BNNSNDArrayDescriptor], gradients: [BNNSNDArrayDescriptor], accumulators: [BNNSNDArrayDescriptor], filterParameters: BNNSFilterParameters?) throws

**Required** Default implementation provided.

## Relationships

### Conforming Types

- BNNS.AdamOptimizer
- BNNS.AdamWOptimizer
- BNNS.RMSPropOptimizer
- BNNS.SGDMomentumOptimizer

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

