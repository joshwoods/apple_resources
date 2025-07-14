

- File Provider
- NSFileProviderManager
-  waitForChanges(below:completionHandler:) 

Instance Method

# waitForChanges(below:completionHandler:)

Requests a notification after the system completes all the specified changes.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func waitForChanges(
    below itemIdentifier: NSFileProviderItemIdentifier,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func waitForChanges(below itemIdentifier: NSFileProviderItemIdentifier) async throws
```

## Parameters 

`itemIdentifier`  

The item’s identifier.

`completionHandler`  

A block that the system calls after all the changes are complete. The block takes the following parameters:

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func waitForChanges(below itemIdentifier: NSFileProviderItemIdentifier) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method waits for all the changes to the item’s descendants to complete before calling the completion handler. If an error occurs during this process, the system immediately passes the error to the completion handler, and you can’t assume all the changes have completed.

Note

The system doesn’t wait for changes to the item specified by the `itemIdentifier` parameter. It only waits for changes to the item’s children. As a result, you can use this method inside a call to modifyItem(_:baseVersion:changedFields:contents:options:request:completionHandler:).

If the `itemIdentifier` property doesn’t refer to a directory, this method immediately calls the completion handler.

## See Also

### Performing actions

class func placeholderURL(for: URL) -> URL

Returns a placeholder URL for a given document URL.

class func writePlaceholder(at: URL, withMetadata: NSFileProviderItem) throws

Writes a document placeholder with the provided metadata.

func register(URLSessionTask, forItemWithIdentifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Registers the URL session task responsible for the specified item.

func signalEnumerator(for: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Alerts the system to changes in the specified folder’s content.

func globalProgress(for: Progress.FileOperationKind) -> Progress

Returns a progress object that tracks either the uploading or downloading of items from the File Provider extension’s remote storage.

