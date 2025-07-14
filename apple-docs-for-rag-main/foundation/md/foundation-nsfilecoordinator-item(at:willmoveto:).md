

- Foundation
- NSFileCoordinator
-  item(at:willMoveTo:) 

Instance Method

# item(at:willMoveTo:)

Announces that your app is moving a file to a new URL.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func item(
    at oldURL: URL,
    willMoveTo newURL: URL
)
```

## Parameters 

`oldURL`  

The old location of the file or directory.

`newURL`  

The new location of the file or directory.

## Discussion

This method is intended for apps that adopt App Sandbox.

Some apps need to rename files while saving them. For example, when a user adds an attachment to a rich text document, TextEdit changes the document’s filename extension from `.rtf` to `.rtfd`. In such a case, in a sandboxed app, you must call this method to declare your intent to rename a file without user approval.

After the renaming process succeeds, call the item(at:didMoveTo:) method, with the same arguments, to provide your app with continued access to the file under its new name, while also giving up access to any file that appears with the old name.

If your macOS app is not sandboxed, this method serves no purpose. This method is nonfunctional in iOS.

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

func item(at: URL, didMoveTo: URL)

Notifies relevant file presenters that the location of a file or directory changed.

func cancel()

Cancels any active file coordination calls.

