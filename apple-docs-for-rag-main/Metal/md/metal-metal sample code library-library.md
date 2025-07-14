

- Metal
-  Metal Sample Code Library 

# Metal Sample Code Library

Explore the complete set of Metal samples.

## Overview

Browse the topics below to find samples relevant to a concept you want to learn more about, starting with the basic computation and render workflows. The samples in the lighting and multiple technique sections demonstrate how to take advantage of the unique GPU architecture of Apple silicon.

## Topics

### Compute Workflows

Performing Calculations on a GPU

Use Metal to find GPUs and perform calculations on them.

Selecting Device Objects for Compute Processing

Switch dynamically between multiple GPUs to efficiently execute a compute-intensive simulation.

Customizing a TensorFlow operation

Implement a custom operation that uses Metal kernels to accelerate neural-network training performance.

Customizing a PyTorch operation

Implement a custom operation in PyTorch that uses Metal kernels to improve performance.

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

Adjusting the level of detail using Metal mesh shaders

Choose and render meshes with several levels of detail using object and mesh shaders.

Creating a 3D application with Hydra rendering

Build a 3D application that integrates with Hydra and USD.

Culling occluded geometry using the visibility result buffer

Draw a scene without rendering hidden geometry by checking whether each object in the scene is visible.

Improving edge-rendering quality with multisample antialiasing (MSAA)

Use Metal’s MSAA to enhance the rendering of edges with custom resolve options and immediate and tile-based resolve paths.

Achieving smooth frame rates with Metal’s display link

Pace rendering with minimal input latency while providing essential information to the operating system for power-efficient rendering, thermal mitigation, and the scheduling of sustainable workloads.

### Textures

Processing a Texture in a Compute Function

Perform parallel calculations on structured data by placing the data in textures.

Reading Pixel Data from a Drawable Texture

Access texture data from the CPU by copying it to a buffer.

Creating and Sampling Textures

Load image data into a texture and apply it to a quadrangle.

Streaming large images with Metal sparse textures

Limit texture memory usage for large textures by loading or unloading image detail on the basis of MIP and tile region.

### Argument Buffers

Managing groups of resources with argument buffers

Create argument buffers to organize related resources.

Using Argument Buffers with Resource Heaps

Reduce CPU overhead by using arrays inside argument buffers and combining them with resource heaps.

Encoding Argument Buffers on the GPU

Use a compute pass to encode an argument buffer and access its arguments in a subsequent render pass.

Rendering Terrain Dynamically with Argument Buffers

Use argument buffers to render terrain in real time with a GPU-driven pipeline.

### Shaders

Creating a Metal Dynamic Library

Compile a library of shaders and write it to a file as a dynamically linked library.

Using Function Specialization to Build Pipeline Variants

Create pipelines for different levels of detail from a common shader source.

### Synchronization

Synchronizing CPU and GPU Work

Avoid stalls between CPU and GPU work by using multiple instances of a resource.

Implementing a Multistage Image Filter Using Heaps and Events

Use events to synchronize access to resources allocated on a heap.

Implementing a Multistage Image Filter Using Heaps and Fences

Use fences to synchronize access to resources allocated on a heap.

### Lighting Techniques

Rendering a Scene with Forward Plus Lighting Using Tile Shaders

Implement a forward plus renderer using the latest features on Apple GPUs.

Rendering a Scene with Deferred Lighting in Objective-C

Avoid expensive lighting calculations by implementing a deferred lighting renderer optimized for immediate mode and tile-based deferred renderer GPUs.

Rendering a Scene with Deferred Lighting in Swift

Avoid expensive lighting calculations by implementing a deferred lighting renderer optimized for immediate mode and tile-based deferred renderer GPUs.

Rendering a Scene with Deferred Lighting in C++

Avoid expensive lighting calculations by implementing a deferred lighting renderer optimized for immediate mode and tile-based deferred renderer GPUs.

Rendering Reflections with Fewer Render Passes

Use layer selection to reduce the number of render passes needed to generate an environment map.

### Multiple Techniques

Modern Rendering with Metal

Use advanced Metal features such as indirect command buffers, sparse textures, and variable rate rasterization to implement complex rendering techniques.

Encoding Indirect Command Buffers on the GPU

Maximize CPU to GPU parallelization by generating render commands on the GPU.

### Ray Tracing

Rendering reflections in real time using ray tracing

Implement realistic real-time lighting by dynamically generating reflection maps by encoding a ray-tracing compute pass.

Accelerating ray tracing using Metal

Implement ray-traced rendering using GPU-based parallel processing.

Control the Ray Tracing Process Using Intersection Queries

Explicitly enumerate a ray’s intersections with acceleration structures by creating an intersection query object.

Accelerating ray tracing and motion blur using Metal

Generate ray-traced images with motion blur using GPU-based parallel processing.

Rendering a curve primitive in a ray tracing scene

Implement ray traced rendering using GPU-based parallel processing.

### HDR

Processing HDR Images with Metal

Implement a post-processing pipeline using the latest features on Apple GPUs.

### OpenGL

Migrating OpenGL Code to Metal

Replace your app’s deprecated OpenGL code with Metal.

Mixing Metal and OpenGL Rendering in a View

Draw with Metal and OpenGL in the same view using an interoperable texture.

