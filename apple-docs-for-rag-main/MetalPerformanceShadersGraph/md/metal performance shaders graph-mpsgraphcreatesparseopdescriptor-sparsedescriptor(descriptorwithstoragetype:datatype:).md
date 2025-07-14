

- Metal Performance Shaders Graph
- MPSGraphCreateSparseOpDescriptor
-  sparseDescriptor(descriptorWithStorageType:dataType:) 

Type Method

# sparseDescriptor(descriptorWithStorageType:dataType:)

Creates a descriptor for a sparse tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class func sparseDescriptor(
    descriptorWithStorageType sparseStorageType: MPSGraphSparseStorageType,
    dataType: MPSDataType
) -> Self?
```

## Parameters 

`sparseStorageType`  

A sparseStorageType.

`dataType`  

A dataType of the sparse tensor.

## Return Value

The descriptor.

