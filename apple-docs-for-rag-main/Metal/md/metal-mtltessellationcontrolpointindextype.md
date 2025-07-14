

- Metal
-  MTLTessellationControlPointIndexType 

Enumeration

# MTLTessellationControlPointIndexType

Options for specifying the size of the control point indices in a control point index buffer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
enum MTLTessellationControlPointIndexType
```

## Topics

### Constants

case none

No size. This value should only be used when drawing patches without a control point index buffer.

case uint16

The size of a 16-bit unsigned integer.

case uint32

The size of a 32-bit unsigned integer.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying Tessellation State

var maxTessellationFactor: Int

The maximum tessellation factor that the tessellator uses when tessellating patches.

var isTessellationFactorScaleEnabled: Bool

A Boolean value that determines whether the pipeline scales the tessellation factor.

var tessellationFactorFormat: MTLTessellationFactorFormat

The format of the tessellation factors in the tessellation factor buffer.

var tessellationControlPointIndexType: MTLTessellationControlPointIndexType

The size of the control point indices in a control point index buffer.

var tessellationFactorStepFunction: MTLTessellationFactorStepFunction

The step function for determining the tessellation factors for a patch from the tessellation factor buffer.

var tessellationOutputWindingOrder: MTLWinding

The winding order of triangles from the tessellator.

var tessellationPartitionMode: MTLTessellationPartitionMode

The partitioning mode that the tessellator uses to derive the number and spacing of segments for subdividing a corresponding edge.

enum MTLTessellationFactorFormat

Options for specifying the format of the tessellation factors in a tessellation factor buffer.

enum MTLTessellationFactorStepFunction

Options for specifying the step function that determines the tessellation factors for a patch from the tessellation factor buffer.

enum MTLTessellationPartitionMode

Options for choosing the partition mode that the tessellator applies when deriving the number and spacing of segments for subdividing a corresponding edge.

