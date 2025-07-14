

- Metal Performance Shaders Graph
- MPSGraphRandomOpDescriptor
-  dataType 

Instance Property

# dataType

The data type of the generated result values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var dataType: MPSDataType { get set }
```

## Discussion

When sampling from the uniform distribution, valid types are MPSDataTypeFloat16, MPSDataTypeFloat32, and MPSDataTypeInt32. When sampling from the normal or truncated normal distribution, valid types are MPSDataTypeFloat16 and MPSDataTypeFloat32.

