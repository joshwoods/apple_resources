

- Metal
-  Ray Tracing with Acceleration Structures 

API Collection

# Ray Tracing with Acceleration Structures

Build a representation of your scene’s geometry using triangles and bounding volumes to quickly trace rays through the scene.

## Overview

Ray tracing can improve your content’s realism by more accurately modeling the behavior of light than traditional rendering. You can also use ray tracing to implement similar techniques that rely on line-of-sight, such as sound obstruction or visually based AI functions.

To apply ray tracing in your app:

1.  Create acceleration structures that represent objects in a scene.

2.  Define a ray’s behavior when it collides into parts of an acceleration structure by creating either intersectors or intersection queries.

3.  Generate rays into the scene from a new or existing shader.

An *intersector* uses a table of your intersection functions that define the custom behavior for each intersection type. An *intersection query* returns to your calling function to handle the custom behavior for all intersection types.

Intersectors work with compute kernels on all GPUs, and with render shaders only on Apple silicon GPUs. Alternatively, your app can use intersection queries on non-Apple GPUs, or for porting code from other graphics APIs.

## Topics

### Ray Tracing Samples

Accelerating ray tracing using Metal

Implement ray-traced rendering using GPU-based parallel processing.

Control the Ray Tracing Process Using Intersection Queries

Explicitly enumerate a ray’s intersections with acceleration structures by creating an intersection query object.

Rendering reflections in real time using ray tracing

Implement realistic real-time lighting by dynamically generating reflection maps by encoding a ray-tracing compute pass.

Rendering a curve primitive in a ray tracing scene

Implement ray traced rendering using GPU-based parallel processing.

### Acceleration Structures

Improving Ray-Tracing Data Access Using Per-Primitive Data

Simplify data access and improve GPU utilization by storing custom primitive data directly in the acceleration structure.

protocol MTLAccelerationStructure

A collection of model data for GPU-accelerated intersection of rays with the model.

class MTLAccelerationStructureDescriptor

A base class for classes that define the configuration for a new acceleration structure.

class MTLPrimitiveAccelerationStructureDescriptor

A description of an acceleration structure that contains geometry primitives.

class MTLInstanceAccelerationStructureDescriptor

A description of an acceleration structure that derives from instances of primitive acceleration structures.

protocol MTLAccelerationStructureCommandEncoder

An object for encoding commands that build or refit acceleration structures.

struct MTLAccelerationStructureUsage

Options that describe which tasks you can perform on an acceleration structure and how the system performs those tasks.

struct MTLAccelerationStructureRefitOptions

### Acceleration Structures Passes

class MTLAccelerationStructurePassDescriptor

class MTLAccelerationStructurePassSampleBufferAttachmentDescriptor

class MTLAccelerationStructurePassSampleBufferAttachmentDescriptorArray

### Geometry Descriptors

class MTLAccelerationStructureGeometryDescriptor

A base class for descriptors that contain geometry data to convert into a ray-tracing acceleration structure.

class MTLAccelerationStructureTriangleGeometryDescriptor

A description of a list of triangle primitives to turn into an acceleration structure.

class MTLAccelerationStructureCurveGeometryDescriptor

enum MTLCurveType

enum MTLCurveBasis

enum MTLCurveEndCaps

class MTLAccelerationStructureBoundingBoxGeometryDescriptor

A description of a list of bounding boxes to turn into an acceleration structure.

### Motion Geometry Descriptors

class MTLAccelerationStructureMotionTriangleGeometryDescriptor

A description of a list of triangle primitives, as motion keyframe data, to turn into an acceleration structure.

class MTLAccelerationStructureMotionCurveGeometryDescriptor

class MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor

A description of a list of bounding boxes, as motion keyframe data, to turn into an acceleration structure.

class MTLMotionKeyframeData

Geometry data for a specific keyframe to use in a moving object.

### Instance Descriptors

struct MTLAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure.

struct MTLAccelerationStructureUserIDInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure, with the instance including a user identifier for the instance.

struct MTLAccelerationStructureMotionInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure, with the instance including a user identifier and motion data for the instance.

struct MTLAccelerationStructureInstanceOptions

Options for adjusting the behavior of an instanced acceleration structure.

class MTLIndirectInstanceAccelerationStructureDescriptor

A description of an acceleration structure that Metal derives from instances of primitive acceleration structures that the GPU can populate.

struct MTLIndirectAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure that the GPU can populate.

struct MTLIndirectAccelerationStructureMotionInstanceDescriptor

A description of an instance in an acceleration structure that the GPU can populate, with motion data for the instance.

### Intersection Function Tables

protocol MTLIntersectionFunctionTable

A table of intersection functions that Metal calls to perform ray-tracing intersection tests.

class MTLIntersectionFunctionTableDescriptor

A specification of how to create an intersection function table.

class MTLIntersectionFunctionDescriptor

A description of an intersection function that performs an intersection test.

struct MTLIntersectionFunctionSignature

Constants for specifying different types of custom intersection functions.

### Supporting Types

typealias MTLAxisAlignedBoundingBox

The bounds for an axis-aligned bounding box.

typealias MTLPackedFloat3

A structure that contains three 32-bit floating-point values with no additional padding.

typealias MTLPackedFloat4x3

A structure that contains the top three rows of a 4x4 matrix of 32-bit floating-point values, in column-major order.

func MTLPackedFloat3Make(Float, Float, Float) -> MTLPackedFloat3

Returns a new packed vector with three floating-point values.

## See Also

### Command Encoders

Render Passes

Encode a render pass to draw graphics into an image.

Compute Passes

Encode a compute pass that runs computations in parallel on a thread grid, processing and manipulating Metal resource data on multiple cores of a GPU.

Blit Passes

Encode a block information transfer pass to adjust and copy data to and from GPU resources, such as buffers and textures.

Indirect Command Encoding

Store draw commands in Metal buffers and run them at a later time on the GPU, either once or repeatedly.

