

- Xcode
- Debugging
- Metal debugger
-  Inspecting sampler states 

Article

# Inspecting sampler states

Verify your sampler state configurations by examining their properties.

## Overview

The Metal debugger allows you to inspect a sampler state with the Sampler State viewer. After opening a sampler state, you can view its associated properties and preview the sampling behavior. For more information, see Inspecting the bound resources for a command or Analyzing memory usage.

### Navigate your sampler state

The Sampler State viewer shows the properties of your sampler state on the left (as configured by MTLSamplerDescriptor) and a preview on the right. The preview illustrates how pixels in a texture appear when using your sampler state.

The square region in the center of the preview corresponds to UV coordinates within the range of `0.0` to `1.0`.

You can use the preview to quickly verify the configuration for your sampler state. For example, if you want a texture to mirror, but it’s drawing a constant value instead, you can check the sampler state. In the screenshot below, the sampler state is configured to clamp to a border color that’s opaque black, rather than using mirror repeat as the address mode:

### Try various combinations

The properties you configure when creating a sampler state determine how a texture looks when sampling it. The properties related to filtering control how pixels combine when the sample footprint is either larger or smaller than a pixel, or when it’s between mipmap levels. The address mode determines the texture coordinate at each pixel when a read falls outside the bounds of a texture. You can try using different combinations of filtering and addressing modes until you achieve your desired look.

| Properties | Preview |
|----|----|
| MTLSamplerMinMagFilter.nearest, MTLSamplerAddressMode.clampToEdge |  |
| MTLSamplerMinMagFilter.nearest, MTLSamplerAddressMode.mirrorClampToEdge |  |
| MTLSamplerMinMagFilter.nearest, MTLSamplerAddressMode.repeat |  |
| MTLSamplerMinMagFilter.nearest, MTLSamplerAddressMode.mirrorRepeat |  |
| MTLSamplerMinMagFilter.nearest, MTLSamplerAddressMode.clampToZero |  |
| MTLSamplerMinMagFilter.nearest, MTLSamplerAddressMode.clampToBorderColor, MTLSamplerBorderColor.opaqueBlack |  |
| MTLSamplerMinMagFilter.nearest, MTLSamplerAddressMode.clampToBorderColor, MTLSamplerBorderColor.opaqueWhite |  |
| MTLSamplerMinMagFilter.nearest, MTLSamplerAddressMode.clampToBorderColor, MTLSamplerBorderColor.transparentBlack |  |
| MTLSamplerMinMagFilter.linear, MTLSamplerAddressMode.clampToEdge |  |
| MTLSamplerMinMagFilter.linear, MTLSamplerAddressMode.clampToEdge |  |
| MTLSamplerMinMagFilter.linear, MTLSamplerAddressMode.repeat |  |
| MTLSamplerMinMagFilter.linear, MTLSamplerAddressMode.mirrorRepeat |  |
| MTLSamplerMinMagFilter.linear, MTLSamplerAddressMode.clampToZero |  |
| MTLSamplerMinMagFilter.linear, MTLSamplerAddressMode.clampToBorderColor, MTLSamplerBorderColor.opaqueBlack |  |
| MTLSamplerMinMagFilter.linear, MTLSamplerAddressMode.clampToBorderColor, MTLSamplerBorderColor.opaqueWhite |  |
| MTLSamplerMinMagFilter.linear, MTLSamplerAddressMode.clampToBorderColor, MTLSamplerBorderColor.transparentBlack |  |

## See Also

### Metal resource inspection

Inspecting acceleration structures

Reveal ray intersection bottlenecks by examining your acceleration structures.

Inspecting buffers

Confirm your buffer formats by examining buffer content.

Inspecting pipeline states

Determine how your render and compute passes behave by examining their properties.

Inspecting shaders

Improve your app’s shader performance by examining and editing your shaders.

Inspecting textures

Discover issues in your textures by examining their content.

