

- Foundation
- NSFileCoordinator
-  item(at:didMoveTo:) 

Instance Method

# item(at:didMoveTo:)

Notifies relevant file presenters that the location of a file or directory changed.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func item(
    at oldURL: URL,
    didMoveTo newURL: URL
)
```

## Parameters 

`oldURL`  

The old location of the file or directory.

`newURL`  

The new location of the file or directory.

## Discussion

If you move or rename a file or directory as part of a write operation, call this method to notify relevant file presenters that the change occurred. This method calls the presentedItemDidMove(to:) method for any of the item’s file presenters. If the item is a directory, this method calls presentedItemDidMove(to:) on the file presenters for the item’s contents. Finally, it calls presentedSubitem(at:didMoveTo:) on the file presenter of any directory containing the item.

You must call this method from a coordinated write block. Calling this method with the same URL in the `oldURL` and `newURL` parameters is harmless. This call must balance a call to item(at:willMoveTo:).

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

func cancel()

Cancels any active file coordination calls.

