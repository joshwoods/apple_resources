

- Metal
- MTLCommandBuffer
-  commit() 

Instance Method

# commit()

Submits the command buffer to run on the GPU.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func commit()
```

**Required**

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

The commit() method sends the command buffer to the MTLCommandQueue instance that owns it, which then schedules it to run on the GPU. If your app calls commit() for a command buffer that isn’t enqueued, the method effectively calls enqueue() for you.

The commit() method has several restrictions, including:

- You can commit a command buffer to its command queue only one time.

- You can only commit a command buffer when it doesn’t have an active encoder (see MTLCommandBuffer and MTLCommandEncoder).

- You can’t encode additional commands to a command buffer after you commit it.

- You can’t call the addScheduledHandler(_:) or addCompletedHandler(_:) methods after you commit a command buffer.

The GPU starts the command buffer after it starts any command buffers that are ahead of it in the same command queue.

## See Also

### Submitting a Command Buffer

func enqueue()

Reserves the next available place for the command buffer in its command queue.

**Required**

