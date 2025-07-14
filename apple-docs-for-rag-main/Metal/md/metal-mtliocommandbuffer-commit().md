

- Metal
- MTLIOCommandBuffer
-  commit() 

Instance Method

# commit()

Submits the command buffer to the queue for execution on the GPU.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func commit()
```

**Required**

## Discussion

If you haven’t already called enqueue() for the command buffer, the commit() method enqueues it at the next position in the input/output command queue.

You can only commit an input/output command buffer once, after which you can’t encode any additional commands or add more completion handlers to it.

## See Also

### Submitting a Command Buffer

func enqueue()

Reserves a place for the input/output command buffer in the input/output command queue without committing the command buffer.

**Required**

