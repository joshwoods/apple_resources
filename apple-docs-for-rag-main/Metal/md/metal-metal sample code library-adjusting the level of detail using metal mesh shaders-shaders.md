

- Metal
- Metal Sample Code Library
-  Adjusting the level of detail using Metal mesh shaders 

Sample Code

# Adjusting the level of detail using Metal mesh shaders

Choose and render meshes with several levels of detail using object and mesh shaders.

Download

iOS 16.0+iPadOS 16.0+macOS 13.0+Xcode 14.0+

## Overview

Note

This sample code project is associated with WWDC22 session 10162: Transform your geometry with Metal mesh shaders.

### Configure the sample code project

To run this sample, you need Xcode 14 or later, and a physical device that supports MTLGPUFamily.mac2 or MTLGPUFamily.apple7, such as:

- A Mac running macOS 13 or later

- An iOS device with an A15 chip or later running iOS 16 or later

This sample can only run on a physical device because it uses Metal’s mesh shader features, which Simulator doesn’t support.

## See Also

### Render Workflows

Using Metal to Draw a View’s Contents

Create a MetalKit view and a render pass to draw the view’s contents.

Using a Render Pipeline to Render Primitives

Render a simple 2D triangle.

Selecting Device Objects for Graphics Rendering

Switch dynamically between multiple GPUs to efficiently render to a display.

Customizing Render Pass Setup

Render into an offscreen texture by creating a custom render pass.

Creating a Custom Metal View

Implement a lightweight view for Metal rendering that’s customized to your app’s needs.

Calculating Primitive Visibility Using Depth Testing

Determine which pixels are visible in a scene by using a depth texture.

Encoding Indirect Command Buffers on the CPU

Reduce CPU overhead and simplify your command execution by reusing commands.

Implementing Order-Independent Transparency with Image Blocks

Draw overlapping, transparent surfaces in any order by using tile shaders and image blocks.

Loading textures and models using Metal fast resource loading

Stream texture and buffer data directly from disk into Metal resources using fast resource loading.

Creating a 3D application with Hydra rendering

Build a 3D application that integrates with Hydra and USD.

Culling occluded geometry using the visibility result buffer

Draw a scene without rendering hidden geometry by checking whether each object in the scene is visible.

Improving edge-rendering quality with multisample antialiasing (MSAA)

Use Metal’s MSAA to enhance the rendering of edges with custom resolve options and immediate and tile-based resolve paths.

Achieving smooth frame rates with Metal’s display link

Pace rendering with minimal input latency while providing essential information to the operating system for power-efficient rendering, thermal mitigation, and the scheduling of sustainable workloads.

