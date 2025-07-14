

- Metal
- MTLRenderPipelineDescriptor
-  isTessellationFactorScaleEnabled 

Instance Property

# isTessellationFactorScaleEnabled

A Boolean value that determines whether the pipeline scales the tessellation factor.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var isTessellationFactorScaleEnabled: Bool { get set }
```

## Discussion

The default value is false.

If this value is true, a scale factor is applied to the tessellation factors after the patch cull check is performed but before the tessellation factors are clamped to the value of maxTessellationFactor. The scale factor is applied only if the patch is not culled.

## See Also

### Related Documentation

func setTessellationFactorScale(Float)

Configures the scale factor for per-patch tessellation factors.

**Required**

### Specifying Tessellation State

var maxTessellationFactor: Int

The maximum tessellation factor that the tessellator uses when tessellating patches.

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

