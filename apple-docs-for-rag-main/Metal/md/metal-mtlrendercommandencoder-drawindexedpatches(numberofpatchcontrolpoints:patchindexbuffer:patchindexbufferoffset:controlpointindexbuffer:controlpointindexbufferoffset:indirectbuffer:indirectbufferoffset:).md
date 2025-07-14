

- Metal
- MTLRenderCommandEncoder
-  drawIndexedPatches(numberOfPatchControlPoints:patchIndexBuffer:patchIndexBufferOffset:controlPointIndexBuffer:controlPointIndexBufferOffset:indirectBuffer:indirectBufferOffset:) 

Instance Method

# drawIndexedPatches(numberOfPatchControlPoints:patchIndexBuffer:patchIndexBufferOffset:controlPointIndexBuffer:controlPointIndexBufferOffset:indirectBuffer:indirectBufferOffset:)

Encodes a draw command that renders multiple instances of tessellated patches with a control point index buffer and indirect arguments.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.12+tvOS 14.5+visionOS 1.0+

``` source
func drawIndexedPatches(
    numberOfPatchControlPoints: Int,
    patchIndexBuffer: (any MTLBuffer)?,
    patchIndexBufferOffset: Int,
    controlPointIndexBuffer: any MTLBuffer,
    controlPointIndexBufferOffset: Int,
    indirectBuffer: any MTLBuffer,
    indirectBufferOffset: Int
)
```

**Required**

## Parameters 

`numberOfPatchControlPoints`  

The number of control points for each patch, which needs to be in the range `[0, 32]`.

`patchIndexBuffer`  

An MTLBuffer instance that contains the indices to patches.

`patchIndexBufferOffset`  

An integer that represents the location, in bytes, from the start of `patchIndexBuffer` where the patch indices begin.

`controlPointIndexBuffer`  

An MTLBuffer instance that contains the indices to control points.

`controlPointIndexBufferOffset`  

An integer that represents the location, in bytes, from the start of `controlPointIndexBuffer` where the control point indices begin.

`indirectBuffer`  

An MTLBuffer instance with data that matches the layout of the MTLDrawPatchIndirectArguments structure.

`indirectBufferOffset`  

An integer that represents the location, in bytes, from the start of `indirectBuffer` where the indirect arguments structure begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

## Discussion

Indirect drawing methods may help your app avoid expensive latency costs. This is because the command reads arguments from an MTLBuffer instance instead of using the CPU to pass parameters to the command.

The method records the encoder’s current rendering state and resources the command needs as it runs. You can safely change the encoder’s render pipeline state to encode other commands after calling this method. Subsequent changes to the state don’t affect the commands already in the encoder’s MTLCommandBuffer.

## See Also

### Drawing with Indexed Tessellation Patches

func drawIndexedPatches(numberOfPatchControlPoints: Int, patchStart: Int, patchCount: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, controlPointIndexBuffer: any MTLBuffer, controlPointIndexBufferOffset: Int, instanceCount: Int, baseInstance: Int)

Encodes a draw command that renders multiple instances of tessellated patches with a control point index buffer.

**Required**

