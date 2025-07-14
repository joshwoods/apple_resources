

- Metal
- MTLIOCommandBuffer
-  addCompletedHandler(\_:) 

Instance Method

# addCompletedHandler(\_:)

Adds a closure that Metal calls immediately after the GPU finishes executing the commands in the input/output command buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func addCompletedHandler(_ block: @escaping MTLIOCommandBufferHandler)
```

**Required**

## Parameters 

`block`  

A Swift closure or an Objective-C block with your code.

## See Also

### Adding Final Commands

func copyStatus(buffer: any MTLBuffer, offset: Int)

Encodes a command that writes the input/output command buffer’s status to a buffer.

**Required**

