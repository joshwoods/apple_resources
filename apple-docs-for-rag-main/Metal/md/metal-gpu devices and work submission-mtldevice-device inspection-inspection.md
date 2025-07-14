

- Metal
- GPU Devices and Work Submission
- MTLDevice
-  Device Inspection 

API Collection

# Device Inspection

Locate and identify a GPU and the features it supports, and sample its counters.

## Topics

### Checking a GPU Device’s Feature Support

func supportsFamily(MTLGPUFamily) -> Bool

Returns a Boolean value that indicates whether the GPU device supports the feature set of a specific GPU family.

**Required**

enum MTLGPUFamily

Represents the functionality for families of GPUs.

func supportsFeatureSet(MTLFeatureSet) -> Bool

Returns a Boolean value that indicates whether the GPU device supports a specific feature set.

**Required**

Deprecated

enum MTLFeatureSet

The device feature sets that define specific platform, hardware, and software configurations.

Deprecated

### Checking Compute Support

var maxThreadgroupMemoryLength: Int

The maximum threadgroup memory available to a compute kernel, in bytes.

**Required**

var maxThreadsPerThreadgroup: MTLSize

The maximum number of threads along each dimension of a threadgroup.

**Required**

### Checking Render Support

var supportsRaytracing: Bool

A Boolean value that indicates whether the GPU device supports ray tracing.

**Required**

var supportsPrimitiveMotionBlur: Bool

A Boolean value that indicates whether the GPU device supports motion blur for ray tracing.

**Required**

var supportsRaytracingFromRender: Bool

A Boolean value that indicates whether you can call ray-tracing functions from a vertex or fragment shader.

**Required**

var supports32BitMSAA: Bool

A Boolean value that indicates whether the GPU can allocate 32-bit integer texture formats and resolve to 32-bit floating-point texture formats.

**Required**

var supportsPullModelInterpolation: Bool

A Boolean value that indicates whether the GPU can compute multiple interpolations of a fragment function’s input.

**Required**

var supportsShaderBarycentricCoordinates: Bool

A Boolean value that indicates whether the GPU supports barycentric coordinates.

**Required**

func supportsVertexAmplificationCount(Int) -> Bool

Returns a Boolean value that indicates whether the GPU supports an amplification factor.

**Required**

var areProgrammableSamplePositionsSupported: Bool

A Boolean value that indicates whether the GPU supports programmable sample positions.

**Required**

var areRasterOrderGroupsSupported: Bool

A Boolean value that indicates whether the GPU supports raster order groups.

**Required**

var areBarycentricCoordsSupported: Bool

A Boolean value that indicates whether the GPU supports barycentric coordinates.

**Required**

Deprecated

### Checking Texture and Sampler Support

var supports32BitFloatFiltering: Bool

A Boolean value that indicates whether the GPU can filter a texture with a 32-bit floating-point format.

**Required**

var supportsBCTextureCompression: Bool

A Boolean value that indicates whether you can use textures that use BC compression.

**Required**

var isDepth24Stencil8PixelFormatSupported: Bool

A Boolean value that indicates whether a device supports a packed depth-and-stencil pixel format.

**Required**

var supportsQueryTextureLOD: Bool

A Boolean value that indicates whether you can query the texture level of detail from within a shader.

**Required**

var readWriteTextureSupport: MTLReadWriteTextureTier

The GPU device’s texture support tier.

**Required**

### Checking Function Pointer Support

var supportsFunctionPointers: Bool

A Boolean value that indicates whether the GPU device supports pointers to compute kernel functions.

**Required**

var supportsFunctionPointersFromRender: Bool

A Boolean value that indicates whether the GPU device supports pointers to render functions.

**Required**

### Checking a GPU Device’s Memory

var currentAllocatedSize: Int

The total amount of memory, in bytes, the GPU device is using for all of its resources.

**Required**

var recommendedMaxWorkingSetSize: UInt64

An approximation of how much memory, in bytes, this GPU device can allocate without affecting its runtime performance.

**Required**

var hasUnifiedMemory: Bool

A Boolean value that indicates whether the GPU shares all of its memory with the CPU.

**Required**

var maxTransferRate: UInt64

The highest theoretical rate, in bytes per second, the system can copy between system memory and the GPU’s dedicated memory (VRAM).

**Required**

### Sampling a GPU Device’s Counters

var counterSets: [any MTLCounterSet]?

The counter sets supported by the device object.

**Required**

func supportsCounterSampling(MTLCounterSamplingPoint) -> Bool

Returns a Boolean value that indicates whether you can read GPU counters at the specified command boundary.

**Required**

enum MTLCounterSamplingPoint

Options for different times when you can sample GPU counters.

func makeCounterSampleBuffer(descriptor: MTLCounterSampleBufferDescriptor) throws -> any MTLCounterSampleBuffer

Creates a counter sample buffer.

**Required**

### Sampling GPU and CPU Timestamps Simultaneously

func sampleTimestamps() -> (cpu: MTLTimestamp, gpu: MTLTimestamp)

Captures and returns a CPU timestamp and a GPU timestamp from the same moment in time.

### Identifying a GPU Device

var name: String

The full name of the GPU device.

**Required**

var architecture: MTLArchitecture

The architectural details of the GPU device.

**Required**

class MTLArchitecture

A class that contains the architectural details of a GPU device.

var registryID: UInt64

The GPU device’s registry identifier.

**Required**

var location: MTLDeviceLocation

The physical location of the GPU relative to the system.

**Required**

enum MTLDeviceLocation

Indicates the location of the GPU relative to the system it’s connect to.

var locationNumber: Int

A specific GPU position based on its general location.

**Required**

var isLowPower: Bool

A Boolean value that indicates whether the GPU lowers its performance to conserve energy.

**Required**

var isRemovable: Bool

A Boolean value that indicates whether the GPU is removable.

**Required**

var isHeadless: Bool

A Boolean value that indicates whether a GPU device doesn’t have a connection to a display.

**Required**

var peerGroupID: UInt64

The peer group ID the GPU belongs to, if applicable.

**Required**

var peerCount: UInt32

The total number of GPUs in the peer group, if applicable.

**Required**

var peerIndex: UInt32

The unique identifier for a GPU in a peer group.

**Required**

## See Also

### Working with GPU Devices

Work Submission

Create queues that submit work to the GPU or load assets into GPU resources, and indirect command buffers that group your frequent commands together.

Pipeline State Creation

Create pipeline states for render and compute passes, samplers, depth and stencil states, and indirect command buffers.

Resource Creation

Load assets with input/output queues and make various resource instances, such as buffers, textures, acceleration structures, and memory heaps.

Shader Library and Archive Creation

Create static and dynamic shader libraries, and binary shader archives.

