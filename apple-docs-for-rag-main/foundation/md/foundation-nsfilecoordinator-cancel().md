

- Foundation
- NSFileCoordinator
-  cancel() 

Instance Method

# cancel()

Cancels any active file coordination calls.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancel()
```

## Discussion

Use this method to cancel any active calls to coordinate the reading or writing of a file. If the block passed to the file coordination call has not yet been executed—perhaps because the file coordinator is still waiting for a response from other file presenters—the file coordinator method stops waiting for a response, does not execute its block, and returns an error object with the error code NSUserCancelledError. However, if the block is already being executed, the file coordinator method does not return until the block finishes executing.

You can call this method from any thread of your application and it returns immediately without waiting for the file coordinator object to respond. Thus, when this method returns, you cannot assume that the read or write operation occurred or did not occur. (In fact, it is possible for this method to return while the file coordinator is in the middle of executing a block.) If you want to know whether the operation actually occurred, you must track it yourself by setting a flag when the block starts executing or by using some other means.

## See Also

### Coordinating File Operations Synchronously

func coordinate(readingItemAt: URL, options: NSFileCoordinator.ReadingOptions, error: NSErrorPointer, byAccessor: (URL) -> Void)

Initiates a read operation on a single file or directory using the specified options.

func coordinate(writingItemAt: URL, options: NSFileCoordinator.WritingOptions, error: NSErrorPointer, byAccessor: (URL) -> Void)

Initiates a write operation on a single file or directory using the specified options.

func coordinate(readingItemAt: URL, options: NSFileCoordinator.ReadingOptions, writingItemAt: URL, options: NSFileCoordinator.WritingOptions, error: NSErrorPointer, byAccessor: (URL, URL) -> Void)

Initiates a read operation that contains a follow-up write operation.

func coordinate(writingItemAt: URL, options: NSFileCoordinator.WritingOptions, writingItemAt: URL, options: NSFileCoordinator.WritingOptions, error: NSErrorPointer, byAccessor: (URL, URL) -> Void)

Initiates a write operation that involves a secondary write operation.

func prepare(forReadingItemsAt: [URL], options: NSFileCoordinator.ReadingOptions, writingItemsAt: [URL], options: NSFileCoordinator.WritingOptions, error: NSErrorPointer, byAccessor: (() -> Void) -> Void)

Prepare to read or write from multiple files in a single batch operation.

func item(at: URL, willMoveTo: URL)

Announces that your app is moving a file to a new URL.

func item(at: URL, didMoveTo: URL)

Notifies relevant file presenters that the location of a file or directory changed.

