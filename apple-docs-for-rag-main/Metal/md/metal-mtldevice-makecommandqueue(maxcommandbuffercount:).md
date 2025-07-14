

- Metal
- MTLDevice
-  makeCommandQueue(maxCommandBufferCount:) 

Instance Method

# makeCommandQueue(maxCommandBufferCount:)

Creates a queue you use to submit rendering and computation commands to a GPU that has a fixed number of uncompleted command buffers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeCommandQueue(maxCommandBufferCount: Int) -> (any MTLCommandQueue)?
```

**Required**

## Parameters 

`maxCommandBufferCount`  

An integer that sets the maximum number of uncompleted command buffers the queue can allow.

## Return Value

A new MTLCommandQueue instance if the method completed successfully; otherwise `nil`.

## Discussion

A Command queue can only submit commands to the GPU device instance that created it.

## See Also

### Creating Command Queues

func makeCommandQueue() -> (any MTLCommandQueue)?

Creates a queue you use to submit rendering and computation commands to a GPU.

**Required**

