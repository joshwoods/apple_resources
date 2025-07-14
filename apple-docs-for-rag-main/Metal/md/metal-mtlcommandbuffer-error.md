

- Metal
- MTLCommandBuffer
-  error 

Instance Property

# error

A description of an error when the GPU encounters an issue as it runs the command buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var error: (any Error)? { get }
```

**Required**

## Mentioned in 

Preparing Your Metal App to Run in the Background

## Discussion

You typically check this property during development to get more information about a runtime issue. The property remains `nil` unless the GPU can’t successfully run the command buffer.

An error’s userInfo dictionary property contains additional information if the command buffer’s errorOptions property includes encoderExecutionStatus. You can retrieve an MTLCommandBufferEncoderInfo instance from the dictionary by accessing it with MTLCommandBufferEncoderInfoErrorKey.

## See Also

### Getting Error Details

var errorOptions: MTLCommandBufferErrorOption

Settings that determine which information the command buffer records about execution errors, and how it does it.

**Required**

protocol MTLCommandBufferEncoderInfo

A container that provides additional information about a runtime failure a GPU encounters as it runs the commands in a command buffer.

let MTLCommandBufferEncoderInfoErrorKey: String

A key to a command buffer error’s user information dictionary that retrieves additional information about a GPU’s runtime error.

