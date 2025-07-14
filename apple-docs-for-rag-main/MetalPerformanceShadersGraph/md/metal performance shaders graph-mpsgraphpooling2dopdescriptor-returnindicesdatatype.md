

- Metal Performance Shaders Graph
- MPSGraphPooling2DOpDescriptor
-  returnIndicesDataType 

Instance Property

# returnIndicesDataType

Defines the data type for returned indices. Use this in conjunction with maxPooling2DReturnIndices(_:descriptor:name:) API. Currently MPSGraph supports the following datatypes: `MPSDataTypeInt32`. Default value: `MPSDataTypeInt32`.

iOS 15.3+iPadOS 15.3+Mac Catalyst 15.3+macOS 12.2+tvOS 15.3+visionOS 1.0+

``` source
var returnIndicesDataType: MPSDataType { get set }
```

