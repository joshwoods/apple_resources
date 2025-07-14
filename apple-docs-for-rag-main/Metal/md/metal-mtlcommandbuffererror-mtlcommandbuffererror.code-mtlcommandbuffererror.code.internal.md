

- Metal
- MTLCommandBufferError
- MTLCommandBufferError.Code
-  MTLCommandBufferError.Code.internal 

Case

# MTLCommandBufferError.Code.internal

An error code that indicates the Metal framework has an internal problem.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case `internal`
```

## Discussion

The local description contains the underlying error code. You can report the scenario that generated this error code with Feedback Assistant.

## See Also

### Error Codes

case none

An error code that represents the absence of any problems.

case timeout

An error code that indicates the system interrupted and terminated the command buffer because it took more time to execute than the system allows.

case pageFault

An error code that indicates the command buffer generated a page fault the GPU can’t service.

case notPermitted

An error code that indicates a process doesn’t have access to a GPU device.

case outOfMemory

An error code that indicates the GPU device doesn’t have sufficient memory to execute a command buffer.

case invalidResource

An error code that indicates the command buffer has an invalid reference to resource.

case memoryless

An error code that indicates the GPU ran out of one or more of its internal resources that support memoryless render pass attachments.

case deviceRemoved

An error code that indicates a person physically removed the GPU device before the command buffer finished running.

case stackOverflow

An error code that indicates the GPU terminated the command buffer because a kernel function of tile shader used too many stack frames.

static var accessRevoked: MTLCommandBufferError.Code

An error code that indicates the system has revoked the Metal device’s access because it’s responsible for too many timeouts or hangs.

case none

An error code that represents the absence of any problems.

case timeout

An error code that indicates the system interrupted and terminated the command buffer because it took more time to execute than the system allows.

case pageFault

An error code that indicates the command buffer generated a page fault the GPU can’t service.

case notPermitted

An error code that indicates a process doesn’t have access to a GPU device.

case outOfMemory

An error code that indicates the GPU device doesn’t have sufficient memory to execute a command buffer.

