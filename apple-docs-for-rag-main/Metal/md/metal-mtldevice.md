

- Metal
-  MTLDevice 

Protocol

# MTLDevice

The main Metal interface to a GPU that apps use to draw graphics and run computations in parallel.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLDevice : NSObjectProtocol
```

## Mentioned in 

Finding Multiple GPUs on an Intel-based Mac

Creating Binary Archives from Device-Built Pipeline State Objects

Getting the Default GPU

Sampling GPU Data into Counter Sample Buffers

Improving your game’s graphics performance and settings

## Overview

You can get the default MTLDevice at runtime by calling MTLCreateSystemDefaultDevice() (see Getting the Default GPU). Each Metal device instance represents a GPU and is the main starting point for your app’s interaction with it. With a Metal device instance, you can inspect a GPU’s features and capabilities (see Device Inspection) and create subsidiary type instances with its factory methods.

- Buffers, textures, and other resources store, synchronize, and pass data between the GPU and CPU (see Resource Fundamentals).

- Input/Output command queues efficiently load resources from the file system (see Resource Loading).

- Command queues create command encoders and schedule work for the GPU, including rendering and compute commands (see Render Passes and Compute Passes).

- Pipeline states store render or compute pipeline configurations — which can be expensive to create — so that you can reuse them, potentially many times.

If your app uses more than one GPU (see Multi-GPU Systems), ensure that instances of these types only interact with others from the same device. For example, your app can pass a texture to a command encoder that comes from the same Metal device, but not to another device.

## Topics

### Working with GPU Devices

Device Inspection

Locate and identify a GPU and the features it supports, and sample its counters.

Work Submission

Create queues that submit work to the GPU or load assets into GPU resources, and indirect command buffers that group your frequent commands together.

Pipeline State Creation

Create pipeline states for render and compute passes, samplers, depth and stencil states, and indirect command buffers.

Resource Creation

Load assets with input/output queues and make various resource instances, such as buffers, textures, acceleration structures, and memory heaps.

Shader Library and Archive Creation

Create static and dynamic shader libraries, and binary shader archives.

### Instance Properties

var maximumConcurrentCompilationTaskCount: Int

**Required**

var shouldMaximizeConcurrentCompilation: Bool

**Required**

### Instance Methods

func makeCommandQueue(descriptor: MTLCommandQueueDescriptor) -> (any MTLCommandQueue)?

Creates a command queue with the provided configuration.

**Required**

func makeLogState(descriptor: MTLLogStateDescriptor) throws -> any MTLLogState

Creates a shader log state with the provided configuration.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Locating and Inspecting a GPU Device

Getting the Default GPU

Select the system’s default GPU device on which to run your Metal code.

Detecting GPU Features and Metal Software Versions

Use the device object’s properties to determine how you perform tasks in Metal.

func MTLCreateSystemDefaultDevice() -> (any MTLDevice)?

Returns the device instance Metal selects as the default.

Multi-GPU Systems

Locate and work with internal and external GPUs and their displays, video memory, and performance tradeoffs.

