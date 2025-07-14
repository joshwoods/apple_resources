

- Metal
- MTLCommandBuffer
-  enqueue() 

Instance Method

# enqueue()

Reserves the next available place for the command buffer in its command queue.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func enqueue()
```

**Required**

## Discussion

The enqueue() method adds the command buffer to the MTLCommandQueue instance that owns it, but doesn’t commit the command buffer to run on the GPU. You can call the command buffer’s commit() method at a later time when it’s ready to run on the GPU. You can call a command buffer’s enqueue() method any time before you call commit(), including before, after, or as you encode commands to it.

Note

The command buffer can only reserve a place in its queue a single time; all subsequent enqueue() calls have no effect.

Enqueuing your command buffers first gives you the flexibility to arrange their relative order of execution before encoding commands to any of them. This approach lets you potentially encode each command buffer on a thread, in parallel, instead of encoding them one by one on a single thread. The order in which each worker thread finishes encoding and commits its command buffer doesn’t matter when you enqueue them in order before committing.

## See Also

### Submitting a Command Buffer

func commit()

Submits the command buffer to run on the GPU.

**Required**

