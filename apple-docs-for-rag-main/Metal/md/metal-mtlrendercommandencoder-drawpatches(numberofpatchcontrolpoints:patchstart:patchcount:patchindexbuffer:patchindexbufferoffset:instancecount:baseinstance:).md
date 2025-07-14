

- Metal
- MTLRenderCommandEncoder
-  drawPatches(numberOfPatchControlPoints:patchStart:patchCount:patchIndexBuffer:patchIndexBufferOffset:instanceCount:baseInstance:) 

Instance Method

# drawPatches(numberOfPatchControlPoints:patchStart:patchCount:patchIndexBuffer:patchIndexBufferOffset:instanceCount:baseInstance:)

Encodes a draw command that renders multiple instances of tessellated patches.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func drawPatches(
    numberOfPatchControlPoints: Int,
    patchStart: Int,
    patchCount: Int,
    patchIndexBuffer: (any MTLBuffer)?,
    patchIndexBufferOffset: Int,
    instanceCount: Int,
    baseInstance: Int
)
```

**Required**

## Parameters 

`numberOfPatchControlPoints`  

The number of control points for each patch, which needs to be in the range `[0, 32]`.

`patchStart`  

The first patch the command draws.

`patchCount`  

The number of patches the command draws for each instance.

`patchIndexBuffer`  

An MTLBuffer instance that contains the indices to patches.

`patchIndexBufferOffset`  

An integer that represents the location, in bytes, from the start of `patchIndexBuffer` where the patch indices begin.

`instanceCount`  

The number of times the command draws `patchCount` patches.

`baseInstance`  

The lowest value the command passes to your vertex shader’s parameter with the `instance_id` attribute.

The command assigns each drawing instance a unique `instance_id` value that increases from `baseInstance` through `(baseInstance + instanceCount - 1)`. Your shader can use that value to identify which instance the vertex belongs to.

For more information about the `instance_id` argument attribute for vertex shaders, see the Metal Shading Language Specification (PDF).

## Discussion

The method records the encoder’s current rendering state and resources the command needs as it runs. You can safely change the encoder’s render pipeline state to encode other commands after calling this method. Subsequent changes to the state don’t affect the commands already in the encoder’s MTLCommandBuffer.

## See Also

### Drawing with Tessellation Patches

func drawPatches(numberOfPatchControlPoints: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a draw command that renders multiple instances of tessellated patches with indirect arguments.

**Required**

