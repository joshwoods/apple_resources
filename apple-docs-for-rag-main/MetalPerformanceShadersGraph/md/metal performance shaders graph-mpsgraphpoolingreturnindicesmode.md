

- Metal Performance Shaders Graph
-  MPSGraphPoolingReturnIndicesMode 

Enumeration

# MPSGraphPoolingReturnIndicesMode

The flattening mode for returned indices with max-pooling.

iOS 15.3+iPadOS 15.3+Mac Catalyst 15.3+macOS 12.2+tvOS 15.3+visionOS 1.0+

``` source
enum MPSGraphPoolingReturnIndicesMode
```

## Topics

### Enumeration Cases

case globalFlatten1D

Returns indices flattened in inner most (last) dimension.

case globalFlatten2D

Returns indices flattened in 2 innermost dimensions. eg: HW in NCHW.

case globalFlatten3D

Returns indices flattened in 3 innernost dimensions. eg: HWC in NHWC.

case globalFlatten4D

Returns indices flattened in 4 innermost dimensions.

case localFlatten1D

Returns indices within pooling window, flattened in inner most dimension.

case localFlatten2D

Returns indices within pooling window, flattened in 2 innermost dimensions. eg: HW in NCHW.

case localFlatten3D

Returns indices within pooling window, flattened in 3 innernost dimensions. eg: HWC in NHWC.

case localFlatten4D

Returns indices within pooling window, flattened in 4 innermost dimensions.

case none

No indices returned.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

