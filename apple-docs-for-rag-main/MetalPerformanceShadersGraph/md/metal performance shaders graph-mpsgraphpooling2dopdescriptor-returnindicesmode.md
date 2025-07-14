

- Metal Performance Shaders Graph
- MPSGraphPooling2DOpDescriptor
-  returnIndicesMode 

Instance Property

# returnIndicesMode

Defines the mode for returned indices of maximum values within each pooling window. Use this in conjunction with maxPooling2DReturnIndices(_:descriptor:name:) API. If `returnIndicesMode = MPSGraphPoolingReturnIndicesNone` then only the first result MPSGraph returns from maxPooling2DReturnIndices(_:descriptor:name:) will be valid and using the second result will assert. Default value: `MPSGraphPoolingReturnIndicesNone`.

iOS 15.3+iPadOS 15.3+Mac Catalyst 15.3+macOS 12.2+tvOS 15.3+visionOS 1.0+

``` source
var returnIndicesMode: MPSGraphPoolingReturnIndicesMode { get set }
```

