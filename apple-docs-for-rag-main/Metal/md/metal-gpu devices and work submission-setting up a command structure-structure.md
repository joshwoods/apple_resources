

- Metal
- GPU Devices and Work Submission
-  Setting Up a Command Structure 

Article

# Setting Up a Command Structure

Discover how Metal executes commands on a GPU.

## Overview

In Metal, you send commands to the GPU so it can perform work on your behalf. A command performs the drawing, parallel computation, and resource management work your app requires.

The relationship between Metal apps and the GPU on a device is a client/server model where your app is the client and the GPU is the server. You make requests by sending commands to the GPU that you encapsulate in a command buffer and then add to a command queue. After processing the commands, the GPU notifies your app when it’s ready for more work.

The order that you place commands in command buffers, then enqueue and commit command buffers, affects the perceived order in which Metal executes your commands.

The following sections explain how to set up a command structure to produce the results you want. Some objects you create once and use throughout your app, and others you create specifically to execute a set of commands.

### Create Expensive Shared Objects During Initialization

Create objects that are expensive to allocate during initialization, not in time-critical code paths. Objects that you can share in your code are command queues, pipelines, buffers, and textures. After you initialize these objects, they’re fast to reuse.

#### Make a Command Queue

To make a command queue, call the device’s makeCommandQueue() function.

- Swift
- Objective-C

```
commandQueue = device.makeCommandQueue()
```

```
commandQueue = [device newCommandQueue];
```

Then use the same command queue throughout your app to hold command buffers. The figure below illustrates the command queue that contains command buffers:

#### Make One or More Pipeline Objects

A *pipeline object* tells Metal how to process your commands. The pipeline object encapsulates functions that you write in the Metal shading language. To use a pipeline in your Metal workflow, follow these steps:

1.  Write Metal shader functions that process your data.

2.  Create a pipeline object that contains your shaders.

3.  Set the state of the render or compute pipeline.

4.  Make draw or compute calls.

Metal doesn’t perform your draw or compute calls immediately. Instead, you use an encoder object to insert commands that encapsulate those calls into your command buffer. After you commit the command buffer, Metal sends it to the GPU and uses the active pipeline object to process the commands.

The figure below illustrates the active pipeline on the GPU that contains your custom shader code that processes commands:

### Issue Commands to the GPU

To execute commands on the GPU, follow this process:

1.  Create a command buffer from a command queue.

2.  Create a command encoder using the command buffer.

3.  Add the commands to the command buffer using the command encoder.

4.  Get callbacks when the GPU schedules and executes the commands by setting completion handlers.

5.  Commit the command buffer.

If you’re performing animation as part of a rendering loop, do this for each frame of the animation. You also follow this process to execute one-off image processing, or machine learning tasks.

#### Create a Command Buffer

Create a command buffer by calling makeCommandBuffer() on the command queue.

- Swift
- Objective-C

```
guard let commandBuffer = commandQueue.makeCommandBuffer() else { 
    return 
}
```

```
id  commandBuffer = [commandQueue commandBuffer];
```

For single-threaded apps, create a single command buffer containing the commands. The figure below illustrates the command buffer’s relationship to the commands it contains:

#### Add Commands to the Command Buffer

When you call task-specific functions on an encoder object — like draws or compute operations — the encoder places commands corresponding to those calls in the command buffer. The encoder inserts the commands into the command buffer, including everything the GPU needs to process the task at runtime.

The figure below illustrates a command encoder inserting commands into a command buffer when the app makes a draw call:

You encode actual commands with concrete subclasses of MTLCommandEncoder, depending on your task. For example, use MTLRenderCommandEncoder to issue render commands, and MTLComputeCommandEncoder to issue parallel computation commands. For a complete list of subclasses, see MTLCommandEncoder.

For a complete rendering example, see Using a Render Pipeline to Render Primitives. For a complete parallel processing example, see Processing a Texture in a Compute Function.

#### Commit a Command Buffer

To submit your commands to run on the GPU, commit the command buffer to the GPU.

- Swift
- Objective-C

```
commandBuffer.commit()
```

```
[commandBuffer commit];
```

Committing a command buffer doesn’t run its commands immediately. Instead, Metal schedules the buffer’s commands to run only after you commit prior command buffers that are waiting in the queue. If you don’t explicitly enqueue a command buffer, Metal does that for you when you commit the buffer.

You can’t reuse a buffer after you commit it, but you can receive notifications when Metal schedules and completes the commands, or you can query the buffer’s status. To receive callbacks during this process, use the MTLCommandBuffer addScheduledHandler(_:) and addCompletedHandler(_:) methods.

As much as possible, the perceived order in which Metal executes the commands is the same as the way you order them. Although Metal might reorder some of your commands before processing them, this usually only occurs when there’s a performance gain and no other perceivable impact.

## See Also

### Submitting Work to a GPU

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

