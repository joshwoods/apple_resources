

- Metal
-  MTLCommandBufferError 

Structure

# MTLCommandBufferError

The command buffer error codes that indicate why the GPU doesn’t finish executing a command buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
struct MTLCommandBufferError
```

## Topics

### Errors Codes

static var none: MTLCommandBufferError.Code

An error code that represents the absence of any problems.

static var timeout: MTLCommandBufferError.Code

An error code that indicates the system interrupted and terminated the command buffer because it took more time to execute than the system allows.

static var pageFault: MTLCommandBufferError.Code

An error code that indicates the command buffer generated a page fault the GPU can’t service.

static var notPermitted: MTLCommandBufferError.Code

An error code that indicates a process doesn’t have access to a GPU device.

static var outOfMemory: MTLCommandBufferError.Code

An error code that indicates the GPU device doesn’t have sufficient memory to execute a command buffer.

static var invalidResource: MTLCommandBufferError.Code

An error code that indicates the command buffer has an invalid reference to resource.

static var memoryless: MTLCommandBufferError.Code

An error code that indicates the GPU ran out of one or more of its internal resources that support memoryless render pass attachments.

static var deviceRemoved: MTLCommandBufferError.Code

An error code that indicates a person physically removed the GPU device before the command buffer finished running.

static var stackOverflow: MTLCommandBufferError.Code

An error code that indicates the GPU terminated the command buffer because a kernel function of tile shader used too many stack frames.

static var accessRevoked: MTLCommandBufferError.Code

An error code that indicates the system has revoked the Metal device’s access because it’s responsible for too many timeouts or hangs.

static var `internal`: MTLCommandBufferError.Code

An error code that indicates the Metal framework has an internal problem.

enum Code

Error codes that indicate why a GPU is unable to finish running a command buffer.

### Error Domain

static var errorDomain: String

The current command buffer error domain.

let MTLCommandBufferErrorDomain: String

The domain for Metal command buffer errors.

### Deprecated

static var blacklisted: MTLCommandBufferError.Code

A former error code that indicates the system has revoked the Metal device’s access because it’s responsible for too many timeouts or hangs.

Deprecated

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

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

protocol MTLCommandEncoder

An encoder that writes GPU commands into a command buffer.

