

- Metal
- Render Passes
-  Rendering to Multiple Texture Slices in a Draw Command 

Article

# Rendering to Multiple Texture Slices in a Draw Command

Select a destination texture slice in your vertex shader.

## Overview

Using layer selection, you can render to multiple layers (*slices*) of a texture array, cube texture, or 3D texture, choosing a destination slice for each primitive in your vertex shader. A layer is a single 1D, 2D, or 3D block of pixels, specified by a slice and mipmap level in the target texture. Load and store actions apply to every slice of the render pass’s attachments.

Layer selection is useful when you need to render content to multiple related textures from the same source data, such as when rendering environment cube maps or stereo imagery for virtual reality.

For a specific example that demonstrates layer selection, see Rendering Reflections with Fewer Render Passes.

### Check Whether the Device Object Supports Layer Selection

All GPUs in the macOS family support layer selection. Layer selection is available in the Apple GPU family starting with family 5. Test for layer selection using the following code:

- Swift
- Objective-C

```
func supportsLayerSelection() -> Bool {
    return device.supportsFamily(MTLGPUFamily.mac2) || device.supportsFamily(MTLGPUFamily.apple5)
}
```

```
- (Boolean) supportsLayerSelection
{
  return
    [_device supportsFamily: MTLGPUFamilyMac1 ] ||
    [_device supportsFamily: MTLGPUFamilyApple5 ];
}
```

### Add Layer Selection to Your Vertex Shader

To specify which slice to render a primitive into, add a vertex output with the `[[render_target_array_index]]` attribute. Your vertex shader must set this value so that Metal knows which slice to render into.

The example below uses instanced rendering to render primitives into multiple output slices. It adds a `layer` field to the vertex output to specify the target slice. The code passes the target in as part of the per-instance properties, and copies it to the vertex output.

```
typedef struct
{
    ...
    uint   layer [[render_target_array_index]];
} ColorInOut;

vertex ColorInOut vertexTransform (
          const Vertex in                               [[ stage_in ]],
          const uint   instanceId                       [[ instance_id ]],
          const device InstanceParams* instanceParams   [[ buffer ]],
{
    ColorInOut out;
    out.layer = instanceParams[instanceId].layer;
    ...
}
```

Your vertex function must return the same index for all vertices that make up any given primitive.

### Configure the Pipeline State Object

Render pipelines that can render to layers must specify the type of primitive that they can render. This requirement differs from a normal render pipeline, where you can select a different primitive for each draw command.

When you configure the MTLRenderPipelineDescriptor for the render pipeline, set the inputPrimitiveTopology property to specify the primitive type it can render.

- Swift
- Objective-C

```
let descriptor = MTLRenderPipelineDescriptor()
descriptor.inputPrimitiveTopology = .triangle
descriptor.rasterSampleCount = 1
...
```

```
MTLRenderPipelineDescriptor *descriptor = [[MTLRenderPipelineDescriptor alloc] init];
descriptor.inputPrimitiveTopology = MTLPrimitiveTopologyClassTriangle;
descriptor.rasterSampleCount = 1
...
```

### Configure the Render Pass

When you configure the MTLRenderPassDescriptor, specify a texture array, cube map texture, or 3D texture as the color attachment. You must also set the render pass descriptor’s renderTargetArrayLength property to the maximum number of slices that the shader can choose from. For example, when rendering to a cube map texture, set the length to `6`.

When rendering to texture arrays and cube maps, you can specify multiple attachments and render to all of them simultaneously. You can’t render to multiple attachments if you specify a 3D texture. Here’s an example that sets up the render pass descriptor with one cube map texture for color data and another for depth information:

- Swift
- Objective-C

```
let reflectionPassDesc = MTLRenderPassDescriptor()
reflectionPassDesc.colorAttachments[0].texture = reflectionCubeMap
reflectionPassDesc.depthAttachment.texture = reflectionCubeMapDepth
reflectionPassDesc.renderTargetArrayLength = 6
...
```

```
MTLRenderPassDescriptor* reflectionPassDesc = [MTLRenderPassDescriptor renderPassDescriptor];
reflectionPassDesc.colorAttachments[0].texture    = _reflectionCubeMap;
reflectionPassDesc.depthAttachment.texture        = _reflectionCubeMapDepth;
reflectionPassDesc.renderTargetArrayLength        = 6;
...
```

## See Also

### Optimizing Techniques

Specifying Drawing and Dispatch Arguments Indirectly

Use indirect commands if you don’t know your draw or dispatch call arguments when you encode the command.

Rendering to Multiple Viewports in a Draw Command

Select viewports and their corresponding scissor rectangles in your vertex shader.

