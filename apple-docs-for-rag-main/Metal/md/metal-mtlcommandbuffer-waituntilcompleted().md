

- Metal
- MTLCommandBuffer
-  waitUntilCompleted() 

Instance Method

# waitUntilCompleted()

Blocks the current thread until the GPU finishes executing the command buffer and all of its completion handlers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func waitUntilCompleted()
```

**Required**

## See Also

### Waiting for State Changes

func waitUntilScheduled()

Blocks the current thread until the command queue schedules the buffer.

**Required**

