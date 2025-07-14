

- Metal Performance Shaders Graph
- MPSGraph
-  call(symbolName:inputTensors:outputTypes:name:) 

Instance Method

# call(symbolName:inputTensors:outputTypes:name:)

Creates an operation which invokes another executable.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func call(
    symbolName: String,
    inputTensors: [MPSGraphTensor],
    outputTypes: [MPSGraphType],
    name: String?
) -> [MPSGraphTensor]
```

## Parameters 

`symbolName`  

The unique identifier used to find the executable in the `MPSGraphCompilationDescriptor.callables` directory.

`inputTensors`  

The tensors which are passed as inputs to the executable being invoked.

`outputTypes`  

The expected return types of the executable being invoked.

`name`  

Name of operation.

## Return Value

An array of valid MPSGraphTensor objects representing the return tensors of the invoked executable.

