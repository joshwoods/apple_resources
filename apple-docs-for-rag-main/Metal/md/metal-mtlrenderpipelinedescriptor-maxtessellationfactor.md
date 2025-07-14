

- Metal
- MTLRenderPipelineDescriptor
-  maxTessellationFactor 

Instance Property

# maxTessellationFactor

The maximum tessellation factor that the tessellator uses when tessellating patches.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var maxTessellationFactor: Int { get set }
```

## Discussion

The default value is `16` and the maximum value is `64`. Any value in between must be set according to the partitioning mode specified by the tessellationPartitionMode property:

- For the MTLTessellationPartitionMode.pow2 partitioning mode, the value must be a power of two.

- For the MTLTessellationPartitionMode.integer partitioning mode, the value can be an even or odd number.

- For the MTLTessellationPartitionMode.fractionalOdd or MTLTessellationPartitionMode.fractionalEven partitioning mode, the value must be an even number.

## See Also

### Specifying Tessellation State

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

enum MTLTessellationControlPointIndexType

Options for specifying the size of the control point indices in a control point index buffer.

enum MTLTessellationFactorStepFunction

Options for specifying the step function that determines the tessellation factors for a patch from the tessellation factor buffer.

enum MTLTessellationPartitionMode

Options for choosing the partition mode that the tessellator applies when deriving the number and spacing of segments for subdividing a corresponding edge.

