

- Accelerate
-  BNNSOptimizerStep(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSOptimizerStep(\_:\_:\_:\_:\_:\_:\_:)

Applies a single optimization step to one or more parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSOptimizerStep(
    _ function: BNNSOptimizerFunction,
    _ OptimizerAlgFields: UnsafeRawPointer,
    _ number_of_parameters: Int,
    _ parameters: UnsafeMutablePointer>,
    _ gradients: UnsafeMutablePointer>,
    _ accumulators: UnsafeMutablePointer?>?,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`function`  

The optimization algorithm.

`OptimizerAlgFields`  

A pointer to parameters for optimization function.

`number_of_parameters`  

The number of parameters the step updates.

`parameters`  

An array of pointers to parameter descriptors.

`gradients`  

An array of pointers to gradient descriptors.

`accumulators`  

An array of pointers to accumulator descriptors.

`filter_params`  

The filter runtime parameters.

## Discussion

Use BNNSOptimizerStep(_:_:_:_:_:_:_:) to update a set of parameters using a supplied optimization algorithm.

Important

Parameter, gradient, and accumulator descriptors must have the same sizes and strides and be of type `float`.

For example, the following shows the code required to update the weights data described by `weightsDescriptor` using an Adam optimizer.

```
var weightsDescriptor: BNNSNDArrayDescriptor = ...
var deltaDescriptor: BNNSNDArrayDescriptor = ...
var accumulatorOneDescriptor: BNNSNDArrayDescriptor = ...
var accumulatorTwoDescriptor: BNNSNDArrayDescriptor = ...
var adamFields: BNNSOptimizerAdamFields = ...

withUnsafeMutablePointer(to: &weightsDescriptor) { weightsDescriptorPtr in
    withUnsafePointer(to: &deltaDescriptor) { deltaDescriptorPtr in
        withUnsafeMutablePointer(to: &accumulatorOneDescriptor) { accumulatorOneDescriptorPtr in
            withUnsafeMutablePointer(to: &accumulatorTwoDescriptor) { accumulatorTwoDescriptorPtr in

                var paramaters = [ weightsDescriptorPtr ]
                var gradients = [ deltaDescriptorPtr ]
                var accumulators = [ Optional(accumulatorOneDescriptorPtr),
                                     Optional(accumulatorTwoDescriptorPtr) ]

                let error = withUnsafePointer(to: &adamFields) { adamFieldsPointer in
                    BNNSOptimizerStep(BNNSOptimizerFunctionAdam,
                                      adamFieldsPointer, 1,
                                      &paramaters,
                                      &gradients,
                                      &accumulators,
                                      nil)
                }

                if error != 0 {
                    fatalError("BNNSOptimizerStep failed.")
                }
            }
        }
    }
}

```

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

struct BNNSOptimizerFunction

A structure that contains optimizer functions.

