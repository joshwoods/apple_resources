

- Metal Performance Shaders Graph
- MPSGraphShapedType
-  init(shape:dataType:) 

Initializer

# init(shape:dataType:)

Initializes a shaped type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(
    shape: [NSNumber]?,
    dataType: MPSDataType
)
```

## Parameters 

`shape`  

The shape of the shaped type.

`dataType`  

The dataType of the shaped type.

## Return Value

A valid MPSGraphShapedType, or nil if allocation failure.

