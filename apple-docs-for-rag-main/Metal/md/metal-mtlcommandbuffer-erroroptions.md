

- Metal
- MTLCommandBuffer
-  errorOptions 

Instance Property

# errorOptions

Settings that determine which information the command buffer records about execution errors, and how it does it.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var errorOptions: MTLCommandBufferErrorOption { get }
```

**Required**

## Discussion

The property reflects the errorOptions property of the MTLCommandBufferDescriptor instance at the time you create the command buffer.

## See Also

### Getting Error Details

var error: (any Error)?

A description of an error when the GPU encounters an issue as it runs the command buffer.

**Required**

protocol MTLCommandBufferEncoderInfo

A container that provides additional information about a runtime failure a GPU encounters as it runs the commands in a command buffer.

let MTLCommandBufferEncoderInfoErrorKey: String

A key to a command buffer error’s user information dictionary that retrieves additional information about a GPU’s runtime error.

