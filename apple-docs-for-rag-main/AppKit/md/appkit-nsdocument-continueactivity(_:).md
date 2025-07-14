

- AppKit
- NSDocument
-  continueActivity(\_:) 

Instance Method

# continueActivity(\_:)

Continues to perform the task for a user activity object using a different block.

macOS 10.7+

``` source
@MainActor
func continueActivity(_ block: () -> Void)
```

## Parameters 

`block`  

The block to be invoked.

## Discussion

When AppKit calls performActivity(withSynchronousWaiting:using:) recursively, it may execute this method with the specified block to avoid a deadlock.

If a block that was passed to performActivity(withSynchronousWaiting:using:) is being invoked, this method invokes the passed-in block, having recorded state that makes inner invocations of performActivity(withSynchronousWaiting:using:) not wait. If this method is invoked outside of an invocation of a block passed to performActivity(withSynchronousWaiting:using:), this method simply invokes the passed-in block.

This method is useful when code executed in a block passed to performActivity(withSynchronousWaiting:using:) may also invoke that method. For example, save(withDelegate:didSave:contextInfo:), which uses performActivity(withSynchronousWaiting:using:), uses this around its invocation of runModalSavePanel(for:delegate:didSave:contextInfo:) or save(to:ofType:for:delegate:didSave:contextInfo:) because both of those methods also use performActivity(withSynchronousWaiting:using:). Without the use of this method the inner invocation of performActivity(withSynchronousWaiting:using:) would wait forever.

## See Also

### Performing Tasks Serially

func performSynchronousFileAccess(() -> Void)

Waits for any scheduled file access to complete, then invokes the passed-in block.

func performAsynchronousFileAccess((() -> Void) -> Void)

Waits for any scheduled file access to complete but without blocking the main thread, then invokes the passed-in block.

func performActivity(withSynchronousWaiting: Bool, using: (() -> Void) -> Void)

Waits for any work scheduled by previous invocations of this method to complete, then invokes the passed-in block.

func continueAsynchronousWorkOnMainThread(() -> Void)

Invokes the passed-in block on the main thread.

