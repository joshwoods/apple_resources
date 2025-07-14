

- Metal
-  MTLCommandBufferEncoderInfoErrorKey 

Global Variable

# MTLCommandBufferEncoderInfoErrorKey

A key to a command buffer error’s user information dictionary that retrieves additional information about a GPU’s runtime error.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
let MTLCommandBufferEncoderInfoErrorKey: String
```

## Discussion

You can retrieve an MTLCommandBufferEncoderInfo instance from the userInfo dictionary of a command buffer’s error property.

## See Also

### Getting Error Details

var error: (any Error)?

A description of an error when the GPU encounters an issue as it runs the command buffer.

**Required**

var errorOptions: MTLCommandBufferErrorOption

Settings that determine which information the command buffer records about execution errors, and how it does it.

**Required**

protocol MTLCommandBufferEncoderInfo

A container that provides additional information about a runtime failure a GPU encounters as it runs the commands in a command buffer.

