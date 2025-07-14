

- Metal
- GPU Devices and Work Submission
- MTLCommandBuffer
-  Command Buffer Debugging 

API Collection

# Command Buffer Debugging

Properties and methods for programmatically debugging runtime issues with a command buffer.

## Topics

### Identifying the Command Buffer

var label: String?

An optional name that can help you identify the command buffer.

**Required**

var commandQueue: any MTLCommandQueue

The command queue that creates the command buffer.

**Required**

var device: any MTLDevice

The GPU device that indirectly owns the command buffer because you create it from a command queue the device also owns.

**Required**

### Grouping Commands within a GPU Frame Capture

func pushDebugGroup(String)

Marks the beginning of a debug group and gives it an identifying label, which temporarily replaces the previous group, if applicable.

**Required**

func popDebugGroup()

Marks the end of a debug group and, if applicable, restores the previous group from a stack.

**Required**

### Getting Error Details

var error: (any Error)?

A description of an error when the GPU encounters an issue as it runs the command buffer.

**Required**

var errorOptions: MTLCommandBufferErrorOption

Settings that determine which information the command buffer records about execution errors, and how it does it.

**Required**

protocol MTLCommandBufferEncoderInfo

A container that provides additional information about a runtime failure a GPU encounters as it runs the commands in a command buffer.

let MTLCommandBufferEncoderInfoErrorKey: String

A key to a command buffer error’s user information dictionary that retrieves additional information about a GPU’s runtime error.

### Reading the Runtime Message Logs

var logs: MTLLogContainer

The messages the command buffer records as the GPU runs its commands.

### Checking Scheduling Times on the CPU

var kernelStartTime: CFTimeInterval

The host time, in seconds, when the CPU begins to schedule the command buffer.

**Required**

var kernelEndTime: CFTimeInterval

The host time, in seconds, when the CPU finishes scheduling the command buffer.

**Required**

### Checking Execution Times on the GPU

var gpuStartTime: CFTimeInterval

The host time, in seconds, when the GPU starts command buffer execution.

**Required**

var gpuEndTime: CFTimeInterval

The host time, in seconds, when the GPU finishes execution of the command buffer.

**Required**

### Determining Whether to Maintain Strong References

var retainedReferences: Bool

A Boolean value that indicates whether the command buffer maintains strong references to the resources it uses.

**Required**

## See Also

### Troubleshooting a Command Buffer

var status: MTLCommandBufferStatus

The command buffer’s current state.

**Required**

enum MTLCommandBufferStatus

The discrete states for a command buffer that represent its life cycle stages.

