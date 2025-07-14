

- Metal
- Render Passes
-  Rendering to Multiple Viewports in a Draw Command 

Article

# Rendering to Multiple Viewports in a Draw Command

Select viewports and their corresponding scissor rectangles in your vertex shader.

## Overview

A viewport defines a subsection of the render targets that you want a drawing command to render into. Using viewport selection, you provide multiple viewports for a drawing command, and dynamically choose one of these viewports for each primitive rendered by the drawing command. Viewport selection makes it easier to consolidate rendering to multiple viewports into fewer drawing commands. For example, you might use viewport selection when rendering stereo imagery or other images whose content is rendered to multiple parts of the render target.

### Check the Device Object for Support for Multiple Viewports

All GPUs in the macOS family support multiple viewports. Multiple viewports are available in the Apple GPU family starting with family 5. Test for support using the code below:

- Swift
- Objective-C

```
func supportsMultipleViewports() -> Bool {
    return device.supportsFamily(MTLGPUFamily.mac2) || device.supportsFamily(MTLGPUFamily.apple5)
}
```

```
- (Boolean) supportsMultipleViewports
{
    return [_device supportsFamily: MTLGPUFamilyMac1 ] ||
           [_device supportsFamily: MTLGPUFamilyApple5 ];
}
```

For the maximum number of viewports you can use with each GPU family, see:

- Metal feature set tables (PDF)

- Metal feature set tables (Numbers)

### Add Viewport Selection to Your Vertex Shader

To specify which viewport a primitive should be rendered into, add a vertex output with the `[[viewport_array_index]]` attribute. Your vertex shader must set this value so that Metal knows which viewport to render into.

The example below uses instanced rendering to primitives to multiple viewports. It adds a `viewPort` field to the vertex output to specify the target slice. The target viewport is passed in as part of the per-instance properties, and copied to the vertex output.

```
typedef struct
{
    ...
    uint   viewport [[viewport_array_index]];
} ColorInOut;

vertex ColorInOut vertexTransform (
    const Vertex in [[ stage_in ]],
    const uint   instanceId                       [[ instance_id ]],
    const device InstanceParams* instanceParams   [[ buffer ]],
{
    ColorInOut out;
    out.viewport = instanceParams[instanceId].viewport;
    ...
}
```

Your vertex function must return the same index for all vertices that make up any given primitive.

The rasterization stage uses the selected viewport and associated scissor rectangle to transform the vertex outputs and then passes the data over to the fragment stage. If you need to know which viewport is being rendered to inside your fragment shader, you can reference the same field that you set in the vertex output.

### Specify Viewports and Scissor Rectangles in Your Draw Command

Call setViewports(_:) to specify multiple viewports and setScissorRects(_:) to specify scissor rectangles:

- Swift
- Objective-C

```
renderEncoder.setViewports(viewPortsArray)
renderEncoder.setScissorRects(scissorRectsArray)
```

```
[renderEncoder setViewports:viewPortsArray count:4];
[renderEncoder setScissorRects:scissorRectsArray count:4];
```

Specify the same number of scissor rectangles and viewports. Coordinate your code that encodes render commands with the code in your shaders such that the indices that your shader generates are within the range of provided values.

## See Also

### Optimizing Techniques

Specifying Drawing and Dispatch Arguments Indirectly

Use indirect commands if you don’t know your draw or dispatch call arguments when you encode the command.

Rendering to Multiple Texture Slices in a Draw Command

Select a destination texture slice in your vertex shader.

