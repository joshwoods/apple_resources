

- Metal
-  MTLBuffer 

Protocol

# MTLBuffer

A resource that stores data in a format defined by your app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLBuffer : MTLResource
```

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

Setting Resource Storage Modes

Estimating How Often a Texture Region Is Accessed

Synchronizing a Managed Resource in macOS

Converting a GPU’s Counter Data into a Readable Format

## Overview

A MTLBuffer object can be used only with the MTLDevice that created it. Don’t implement this protocol yourself; instead, use the following MTLDevice methods to create `MTLBuffer` objects:

- makeBuffer(length:options:) creates a `MTLBuffer` object with a new storage allocation.

- makeBuffer(bytes:length:options:) creates a `MTLBuffer` object by copying data from an existing storage allocation into a new allocation.

- makeBuffer(bytesNoCopy:length:options:deallocator:) creates a `MTLBuffer` object that reuses an existing storage allocation and does not allocate any new storage.

The Metal framework doesn’t know anything about the contents of a MTLBuffer, just its size. You define the format of the data in the buffer and ensure that your app and your shaders know how to read and write the data. For example, you might create a struct in your shader that defines the data you want to store in the buffer and its memory layout.

If you create a buffer with a managed resource storage mode (MTLStorageMode.managed), you must call didModifyRange: to tell Metal to copy any changes to the GPU.

## Topics

### Creating a Texture That Shares Buffer Data

func makeTexture(descriptor: MTLTextureDescriptor, offset: Int, bytesPerRow: Int) -> (any MTLTexture)?

Creates a texture that shares its storage with the buffer.

**Required**

### Reading the Buffer’s Data on the CPU

func contents() -> UnsafeMutableRawPointer

Gets the system address of the buffer’s storage allocation.

**Required**

### Synchronizing Data to the GPU for Managed Buffers

func didModifyRange(Range&lt;Int>)

Informs the GPU that the CPU has modified a section of the buffer.

### Debugging Buffers

func addDebugMarker(String, range: Range&lt;Int>)

Adds a debug marker string to a specific buffer range.

func removeAllDebugMarkers()

Removes all debug marker strings from the buffer.

**Required**

### Reading Buffer Length

var length: Int

The logical size of the buffer, in bytes.

**Required**

### Creating Views of Buffers on Other GPUs

func makeRemoteBufferView(any MTLDevice) -> (any MTLBuffer)?

Creates a remote view of the buffer for another GPU in the same peer group.

**Required**

var remoteStorageBuffer: (any MTLBuffer)?

The buffer on another GPU that the buffer was created from, if any.

**Required**

### Instance Properties

var gpuAddress: UInt64

**Required**

## Relationships

### Inherits From

- MTLAllocation
- MTLResource
- NSObjectProtocol

