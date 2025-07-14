

- Metal
- MTLRenderPipelineDescriptor
-  tessellationControlPointIndexType 

Instance Property

# tessellationControlPointIndexType

The size of the control point indices in a control point index buffer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var tessellationControlPointIndexType: MTLTessellationControlPointIndexType { get set }
```

## Discussion

The default value is MTLTessellationControlPointIndexType.none; use this value when drawing patches without a control point index buffer. This value must be either MTLTessellationControlPointIndexType.uint16 or MTLTessellationControlPointIndexType.uint32 when drawing patches with indexed control points.

## See Also

### Related Documentation

func drawIndexedPatches(numberOfPatchControlPoints: Int, patchStart: Int, patchCount: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, controlPointIndexBuffer: any MTLBuffer, controlPointIndexBufferOffset: Int, instanceCount: Int, baseInstance: Int)

Encodes a draw command that renders multiple instances of tessellated patches with a control point index buffer.

**Required**

func drawIndexedPatches(numberOfPatchControlPoints: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, controlPointIndexBuffer: any MTLBuffer, controlPointIndexBufferOffset: Int, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a draw command that renders multiple instances of tessellated patches with a control point index buffer and indirect arguments.

**Required**

### Specifying Tessellation State

var maxTessellationFactor: Int

The maximum tessellation factor that the tessellator uses when tessellating patches.

var isTessellationFactorScaleEnabled: Bool

A Boolean value that determines whether the pipeline scales the tessellation factor.

var tessellationFactorFormat: MTLTessellationFactorFormat

The format of the tessellation factors in the tessellation factor buffer.

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

