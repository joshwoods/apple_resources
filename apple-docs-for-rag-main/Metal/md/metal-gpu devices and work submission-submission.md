

- Metal
-  GPU Devices and Work Submission 

API Collection

# GPU Devices and Work Submission

Find any available GPU, submit work to it with command buffers, suspend work, and coordinate between multiple GPUs.

## Overview

You can use any available GPU’s MTLDevice instance in addition to the default instance that MTLCreateSystemDefaultDevice() returns. For each device instance, get its MTLCommandQueue instance, and create one or more MTLCommandBuffer instances to send work to the GPU.

When the system suspends your app, use the command queue to finish command buffers already in progress. See Preparing Your Metal App to Run in the Background for more information.

## Topics

### Locating and Inspecting a GPU Device

Getting the Default GPU

Select the system’s default GPU device on which to run your Metal code.

Detecting GPU Features and Metal Software Versions

Use the device object’s properties to determine how you perform tasks in Metal.

func MTLCreateSystemDefaultDevice() -> (any MTLDevice)?

Returns the device instance Metal selects as the default.

protocol MTLDevice

The main Metal interface to a GPU that apps use to draw graphics and run computations in parallel.

Multi-GPU Systems

Locate and work with internal and external GPUs and their displays, video memory, and performance tradeoffs.

### Submitting Work to a GPU

Setting Up a Command Structure

Discover how Metal executes commands on a GPU.

protocol MTLCommandQueue

An instance you use to create, submit, and schedule command buffers to a specific GPU device to run the commands within those buffers.

class MTLCommandQueueDescriptor

A configuration that customizes the behavior for a new command queue.

protocol MTLCommandBuffer

A container that stores a sequence of GPU commands that you encode into it.

class MTLCommandBufferDescriptor

A configuration that customizes the behavior for a new command buffer.

struct MTLCommandBufferError

The command buffer error codes that indicate why the GPU doesn’t finish executing a command buffer.

protocol MTLCommandEncoder

An encoder that writes GPU commands into a command buffer.

### Suspending Work on a GPU

Preparing Your Metal App to Run in the Background

Prepare your app to move into the background by pausing future GPU use and ensuring previous work is scheduled.

