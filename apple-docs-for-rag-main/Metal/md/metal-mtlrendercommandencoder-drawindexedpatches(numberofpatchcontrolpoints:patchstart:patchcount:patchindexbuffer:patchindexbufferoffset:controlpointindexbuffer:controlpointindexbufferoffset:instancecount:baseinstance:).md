

- Metal
- MTLRenderCommandEncoder
-  drawIndexedPatches(numberOfPatchControlPoints:patchStart:patchCount:patchIndexBuffer:patchIndexBufferOffset:controlPointIndexBuffer:controlPointIndexBufferOffset:instanceCount:baseInstance:) 

Instance Method

# drawIndexedPatches(numberOfPatchControlPoints:patchStart:patchCount:patchIndexBuffer:patchIndexBufferOffset:controlPointIndexBuffer:controlPointIndexBufferOffset:instanceCount:baseInstance:)

Encodes a draw command that renders multiple instances of tessellated patches with a control point index buffer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func drawIndexedPatches(
    numberOfPatchControlPoints: Int,
    patchStart: Int,
    patchCount: Int,
    patchIndexBuffer: (any MTLBuffer)?,
    patchIndexBufferOffset: Int,
    controlPointIndexBuffer: any MTLBuffer,
    controlPointIndexBufferOffset: Int,
    instanceCount: Int,
    baseInstance: Int
)
```

**Required**

## Parameters 

`numberOfPatchControlPoints`  

The number of control points for each patch, which needs to be in the range `[0, 32]`.

`patchStart`  

The patch start index.

`patchCount`  

The number of patches in each instance.

`patchIndexBuffer`  

An MTLBuffer instance that contains the indices to patches.

`patchIndexBufferOffset`  

An integer that represents the location, in bytes, from the start of `patchIndexBuffer` where the patch indices begin.

`controlPointIndexBuffer`  

An MTLBuffer instance that contains the indices to control points.

`controlPointIndexBufferOffset`  

An integer that represents the location, in bytes, from the start of `controlPointIndexBuffer` where the control point indices begin.

`instanceCount`  

The number of times the command draws `patchCount` patches.

`baseInstance`  

The lowest value the command passes to your vertex shader’s parameter with the `instance_id` attribute.

The command assigns each drawing instance a unique `instance_id` value that increases from `baseInstance` through `(baseInstance + instanceCount - 1)`. Your shader can use that value to identify which instance the vertex belongs to.

For more information about the `instance_id` argument attribute for vertex shaders, see the Metal Shading Language Specification (PDF).

## Discussion

The method records the encoder’s current rendering state and resources the command needs as it runs. You can safely change the encoder’s render pipeline state to encode other commands after calling this method. Subsequent changes to the state don’t affect the commands already in the encoder’s MTLCommandBuffer.

## See Also

### Drawing with Indexed Tessellation Patches

func drawIndexedPatches(numberOfPatchControlPoints: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, controlPointIndexBuffer: any MTLBuffer, controlPointIndexBufferOffset: Int, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a draw command that renders multiple instances of tessellated patches with a control point index buffer and indirect arguments.

**Required**

