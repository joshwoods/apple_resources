

- Metal
- MTLDevice
-  makeCommandQueue() 

Instance Method

# makeCommandQueue()

Creates a queue you use to submit rendering and computation commands to a GPU.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeCommandQueue() -> (any MTLCommandQueue)?
```

**Required**

## Return Value

A new MTLCommandQueue instance if the method completed successfully; otherwise `nil`.

## Mentioned in 

Setting Up a Command Structure

## Discussion

A command queue can only submit commands to the GPU device instance that created it.

Important

The command queues you create with this method allow up to 64 uncompleted command buffers at time.

This method is the equivalent of passing `64` to the makeCommandQueue(maxCommandBufferCount:) method.

- Swift
- Objective-C

```
let commandQueue = device.makeCommandQueue(maxCommandBufferCount: 64)
```

```
id commandQueue;

NSUInteger capacity = 64;
commandQueue = [device newCommandQueueWithMaxCommandBufferCount:capacity];
```

## See Also

### Creating Command Queues

func makeCommandQueue(maxCommandBufferCount: Int) -> (any MTLCommandQueue)?

Creates a queue you use to submit rendering and computation commands to a GPU that has a fixed number of uncompleted command buffers.

**Required**

