

- File Provider
- NSFileProviderExtension
-  itemChanged(at:) 

Instance Method

# itemChanged(at:)

Tells the File Provider extension that a document has changed.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
func itemChanged(at url: URL)
```

## Parameters 

`url`  

The URL of a shared document.

## Discussion

The system calls this method when a shared file’s content changes, typically in response to coordinated writes from the host app.

You must override this method and respond to these changes. Do not call `super` in your implementations.

In your implementation, defer all networking, asynchronous, or long-running operations to background tasks. For networking tasks, create a background URLSession task, and then register the task with the file provider manager by calling the manager’s register(_:forItemWithIdentifier:completionHandler:) method.

## See Also

### Managing shared files

func providePlaceholder(at: URL, completionHandler: ((any Error)?) -> Void)

Triggers the creation of a placeholder for the given URL.

func startProvidingItem(at: URL, completionHandler: ((any Error)?) -> Void)

Provides an actual file on disk for a placeholder.

func stopProvidingItem(at: URL)

Tells the File Provider extension that a given document is no longer being accessed.

