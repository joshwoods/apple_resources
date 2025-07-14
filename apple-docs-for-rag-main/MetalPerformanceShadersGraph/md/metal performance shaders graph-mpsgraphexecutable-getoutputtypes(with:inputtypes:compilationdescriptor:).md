

- Metal Performance Shaders Graph
- MPSGraphExecutable
-  getOutputTypes(with:inputTypes:compilationDescriptor:) 

Instance Method

# getOutputTypes(with:inputTypes:compilationDescriptor:)

Get output shapes for a specialized executable.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
func getOutputTypes(
    with device: MPSGraphDevice?,
    inputTypes: [MPSGraphType],
    compilationDescriptor: MPSGraphCompilationDescriptor?
) -> [MPSGraphShapedType]?
```

## Parameters 

`device`  

Optional MPSGraph device to compile with

`inputTypes`  

Input types expected to be passed to the executable.

`compilationDescriptor`  

CompilationDescriptor to be used to specialize, since the executable was created with a compilationDescriptor already this one overrides those settings to the extent it can.

## Discussion

In case specialization has not been done yet then calling this function will specialize for the given input shapes.

