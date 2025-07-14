

- AppKit
- NSDocument
-  performSynchronousFileAccess(\_:) 

Instance Method

# performSynchronousFileAccess(\_:)

Waits for any scheduled file access to complete, then invokes the passed-in block.

macOS 10.7+

``` source
nonisolated
func performSynchronousFileAccess(_ block: () -> Void)
```

## Parameters 

`block`  

A block that performs file access.

## Discussion

Given a block that will perform file access, this method waits for any file access scheduled by previous invocations of this method or performAsynchronousFileAccess(_:) to complete, then invokes the passed-in block. When the block invocation returns, the method allows the next scheduled file access to to be performed, if any.

Like performActivity(withSynchronousWaiting:using:), this method’s primary use is to wait for asynchronous saving, but in contrast with that method it is only for the part of an asynchronous saving operation that actually touches the document’s file or values in memory that are relative to the document’s file.

In general, you should use this method or performAsynchronousFileAccess(_:) around code that gets or sets values in memory that only make sense in the context of the document file’s current state. For example, `NSDocument` itself consistently uses this mechanism when using the following methods and properties:

- The fileType, fileURL, fileModificationDate, and autosavedContentsFileURL properties, because you can’t reliably make decisions based on a file’s location, type, or modification date when it is being asynchronously moved, renamed, or changed at that moment.

- The isDocumentEdited and hasUnautosavedChanges properties, because you can’t reliably make decisions based on whether the document’s contents in memory have been saved to a file when it is being asynchronously saved at that moment.

- updateChangeCount(withToken:for:) and, sometimes, updateChangeCount(_:), to make using this mechanism when invoking isDocumentEdited and hasUnautosavedChanges meaningful.

## See Also

### Performing Tasks Serially

func performAsynchronousFileAccess((() -> Void) -> Void)

Waits for any scheduled file access to complete but without blocking the main thread, then invokes the passed-in block.

func performActivity(withSynchronousWaiting: Bool, using: (() -> Void) -> Void)

Waits for any work scheduled by previous invocations of this method to complete, then invokes the passed-in block.

func continueActivity(() -> Void)

Continues to perform the task for a user activity object using a different block.

func continueAsynchronousWorkOnMainThread(() -> Void)

Invokes the passed-in block on the main thread.

