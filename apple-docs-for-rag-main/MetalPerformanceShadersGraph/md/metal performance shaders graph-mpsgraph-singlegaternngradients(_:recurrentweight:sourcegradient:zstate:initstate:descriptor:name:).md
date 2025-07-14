

- Metal Performance Shaders Graph
- MPSGraph
-  singleGateRNNGradients(\_:recurrentWeight:sourceGradient:zState:initState:descriptor:name:) 

Instance Method

# singleGateRNNGradients(\_:recurrentWeight:sourceGradient:zState:initState:descriptor:name:)

Creates a single-gate RNN gradient operation and returns the gradient tensor values.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func singleGateRNNGradients(
    _ source: MPSGraphTensor,
    recurrentWeight: MPSGraphTensor,
    sourceGradient: MPSGraphTensor,
    zState: MPSGraphTensor,
    initState: MPSGraphTensor?,
    descriptor: MPSGraphSingleGateRNNDescriptor,
    name: String?
) -> [MPSGraphTensor]
```

## Parameters 

`source`  

A tensor that contains the source data `x[t]` with the data layout \[T,N,I\]. In case `inputWeight = nil` and `bidirectional = NO` then the layout is \[T,N,H\] and for `inputWeight = nil` and `bidirectional = YES` the layout is \[T,N,2H\].

`recurrentWeight`  

A tensor containing the recurrent weights `R`. For `bidirectional` the layout is \[2,H,H\] and otherwise it is \[H,H\]. Note: For `bidirectional` this tensor must have a static shape.

`sourceGradient`  

The input gradient, that is the gradient of a tensor with respect to the first output of the forward pass.

`zState`  

The second output of singleGateRNN(_:recurrentWeight:inputWeight:bias:initState:mask:descriptor:name:) with `descriptor.training = YES`.

`initState`  

The initial internal state of the RNN `h[-1]` - optional, if missing the operation assumes zeroes. For `bidirectional` the layout is \[N,2H\] and otherwise it is \[N,H\].

`descriptor`  

A descriptor that defines the parameters for the RNN operation.

`name`  

The name for the operation.

## Return Value

A valid `MPSGraphTensor` array containing gradients for each input tensor, except for `sourceGradient` and `mask`. In case an input is `nil`, no gradient will be returned for it. The order of the gradients will be: for `source`, for `recurrentWeight`, for `inputWeight`, for `bias` and finally for `initState`.

## Discussion

For details of this operation and parameters, refer to documentation of singleGateRNN(_:recurrentWeight:inputWeight:bias:initState:mask:descriptor:name:).

