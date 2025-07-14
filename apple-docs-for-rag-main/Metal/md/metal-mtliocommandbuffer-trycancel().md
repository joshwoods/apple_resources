

- Metal
- MTLIOCommandBuffer
-  tryCancel() 

Instance Method

# tryCancel()

Submits a request to abandon a command buffer the queue is currently running.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func tryCancel()
```

**Required**

## Discussion

Check the command buffer’s status property after it completes, either after waitUntilCompleted() or in one of your completion handlers (see addCompletedHandler(_:)).

