

- Metal
- MTLCommandBufferError
-  internal 

Type Property

# internal

An error code that indicates the Metal framework has an internal problem.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
static var `internal`: MTLCommandBufferError.Code { get }
```

## Discussion

The local description contains the underlying error code. You can report the scenario that generated this error code with Feedback Assistant.

## See Also

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

enum Code

Error codes that indicate why a GPU is unable to finish running a command buffer.

