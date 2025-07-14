

- File Provider
- NSFileProviderManager
-  register(\_:forItemWithIdentifier:completionHandler:) 

Instance Method

# register(\_:forItemWithIdentifier:completionHandler:)

Registers the URL session task responsible for the specified item.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
func register(
    _ task: URLSessionTask,
    forItemWithIdentifier identifier: NSFileProviderItemIdentifier,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func register(
    _ task: URLSessionTask,
    forItemWithIdentifier identifier: NSFileProviderItemIdentifier
) async throws
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func register(_ task: URLSessionTask, forItemWithIdentifier identifier: NSFileProviderItemIdentifier) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Performing actions

class func placeholderURL(for: URL) -> URL

Returns a placeholder URL for a given document URL.

class func writePlaceholder(at: URL, withMetadata: NSFileProviderItem) throws

Writes a document placeholder with the provided metadata.

func signalEnumerator(for: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Alerts the system to changes in the specified folder’s content.

func waitForChanges(below: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Requests a notification after the system completes all the specified changes.

func globalProgress(for: Progress.FileOperationKind) -> Progress

Returns a progress object that tracks either the uploading or downloading of items from the File Provider extension’s remote storage.

