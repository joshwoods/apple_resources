

- AppKit
- NSDocument
-  continueAsynchronousWorkOnMainThread(\_:) 

Instance Method

# continueAsynchronousWorkOnMainThread(\_:)

Invokes the passed-in block on the main thread.

macOS 10.7+

``` source
nonisolated
func continueAsynchronousWorkOnMainThread(_ block: @escaping () -> Void)
```

## Parameters 

`block`  

The block to be invoked.

## Discussion

If the main thread is blocked by an invocation of performActivity(withSynchronousWaiting:using:) or performSynchronousFileAccess(_:), this method interrupts that blocking activity, performs the specified `block`, and then resumes the blocking activity after `block` returns. Invocations of this method always return before the passed-in block is invoked.

You can invoke this method when work is being done on a non-main thread and part of the work must be continued on the main thread. For example, save(to:ofType:for:completionHandler:) uses this method when it has just completed the actual writing of the file during asynchronous saving and, to finish the saving operation, must invoke updateChangeCount(withToken:for:) and other methods on the main thread.

This method can be invoked on any thread.

## See Also

### Performing Tasks Serially

func performSynchronousFileAccess(() -> Void)

Waits for any scheduled file access to complete, then invokes the passed-in block.

func performAsynchronousFileAccess((() -> Void) -> Void)

Waits for any scheduled file access to complete but without blocking the main thread, then invokes the passed-in block.

func performActivity(withSynchronousWaiting: Bool, using: (() -> Void) -> Void)

Waits for any work scheduled by previous invocations of this method to complete, then invokes the passed-in block.

func continueActivity(() -> Void)

Continues to perform the task for a user activity object using a different block.

