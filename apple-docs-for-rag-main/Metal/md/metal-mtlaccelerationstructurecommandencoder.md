

- Metal
-  MTLAccelerationStructureCommandEncoder 

Protocol

# MTLAccelerationStructureCommandEncoder

An object for encoding commands that build or refit acceleration structures.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLAccelerationStructureCommandEncoder : MTLCommandEncoder
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Overview

Don’t implement this protocol yourself; instead you call methods on an MTLCommandBuffer object to create command encoders. Command encoders are lightweight objects that you re-create every time you need to send commands to the GPU.

## Topics

### Building an Acceleration Structure

func build(accelerationStructure: any MTLAccelerationStructure, descriptor: MTLAccelerationStructureDescriptor, scratchBuffer: any MTLBuffer, scratchBufferOffset: Int)

Encodes a command to build a new acceleration structure.

**Required**

### Copying an Acceleration Structure

func copy(sourceAccelerationStructure: any MTLAccelerationStructure, destinationAccelerationStructure: any MTLAccelerationStructure)

Encodes a command to copy the data from one acceleration structure to another.

**Required**

func writeCompactedSize(accelerationStructure: any MTLAccelerationStructure, buffer: any MTLBuffer, offset: Int)

Encodes a command to calculate the compacted size of an acceleration structure.

**Required**

func writeCompactedSize(accelerationStructure: any MTLAccelerationStructure, buffer: any MTLBuffer, offset: Int, sizeDataType: MTLDataType)

Encodes a command to calculate the compacted size of an acceleration structure, taking into account the size of the output data.

**Required**

func copyAndCompact(sourceAccelerationStructure: any MTLAccelerationStructure, destinationAccelerationStructure: any MTLAccelerationStructure)

Encodes a command to compact an acceleration structure’s data and copy it into a different acceleration structure.

**Required**

### Refitting an Acceleration Structure

func refit(sourceAccelerationStructure: any MTLAccelerationStructure, descriptor: MTLAccelerationStructureDescriptor, destinationAccelerationStructure: (any MTLAccelerationStructure)?, scratchBuffer: (any MTLBuffer)?, scratchBufferOffset: Int)

Updates an acceleration structure with new geometry or instance data.

**Required**

### Synchronizing Command Execution for Untracked Resources

func updateFence(any MTLFence)

Encodes a command that instructs the GPU to update a fence, which signals passes waiting on the fence.

**Required**

func waitForFence(any MTLFence)

Encodes a command that instructs the GPU to pause before starting the acceleration structure commands until another pass updates a fence.

**Required**

### Specifying Resource Usage for Argument Buffers

func useHeap(any MTLHeap)

Makes the resources contained in the specified heap available to the acceleration structure pass.

**Required**

func useHeaps([any MTLHeap])

Makes the resources contained in the specified heaps available to the acceleration structure pass.

func useResource(any MTLResource, usage: MTLResourceUsage)

Makes a resource available to the acceleration structure pass.

**Required**

func useResources([any MTLResource], usage: MTLResourceUsage)

Makes multiple resources available to the acceleration structure pass.

struct MTLResourceUsage

Options that describe how a graphics or compute function uses an argument buffer’s resource.

### Sampling Acceleration Structure Execution Data

func sampleCounters(sampleBuffer: any MTLCounterSampleBuffer, sampleIndex: Int, barrier: Bool)

Encodes a command to sample hardware counters at this point in the acceleration structure pass and store the samples into a counter sample buffer.

**Required**

### Instance Methods

func refit(sourceAccelerationStructure: any MTLAccelerationStructure, descriptor: MTLAccelerationStructureDescriptor, destinationAccelerationStructure: (any MTLAccelerationStructure)?, scratchBuffer: (any MTLBuffer)?, scratchBufferOffset: Int, options: MTLAccelerationStructureRefitOptions)

**Required**

## Relationships

### Inherits From

- MTLCommandEncoder
- NSObjectProtocol

## See Also

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

struct MTLAccelerationStructureUsage

Options that describe which tasks you can perform on an acceleration structure and how the system performs those tasks.

struct MTLAccelerationStructureRefitOptions

