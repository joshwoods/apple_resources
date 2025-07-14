

- Metal Performance Shaders Graph
- MPSGraphExecutable
-  specialize(with:inputTypes:compilationDescriptor:) 

Instance Method

# specialize(with:inputTypes:compilationDescriptor:)

Specialize the executable and optimize it.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func specialize(
    with device: MPSGraphDevice?,
    inputTypes: [MPSGraphType],
    compilationDescriptor: MPSGraphCompilationDescriptor?
)
```

## Parameters 

`device`  

Ooptional MPSGraph device to compile with.

`inputTypes`  

Input types expected to be passed to the executable.

`compilationDescriptor`  

Compilation descriptor to be used to specialize, since the executable was created with a compilationDescriptor already this one overrides those settings to the extent it can.

## Discussion

Use this method to choose when specialization happens, else it occurs at encode time automatically.

