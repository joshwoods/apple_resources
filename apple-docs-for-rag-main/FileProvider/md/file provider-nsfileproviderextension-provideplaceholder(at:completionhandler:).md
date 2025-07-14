

- File Provider
- NSFileProviderExtension
-  providePlaceholder(at:completionHandler:) 

Instance Method

# providePlaceholder(at:completionHandler:)

Triggers the creation of a placeholder for the given URL.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
func providePlaceholder(
    at url: URL,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func providePlaceholder(at url: URL) async throws
```

## Parameters 

`url`  

The URL of a shared document.

`completionHandler`  

A block that the system calls after the placeholder is created.

The completion handler takes the following parameter:

error  
If the placeholder was successfully written to disk, this value is `nil`. Otherwise, it holds an `NSError` object describing the error.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func providePlaceholder(at url: URL) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The system calls this method when it needs a placeholder for a document that’s returned by the File Provider extension, but is not stored locally. Override `providePlaceholder(at:completionHandler:)` to create a placeholder for the given URL. This task can be broken into three steps: looking up the document’s file provider item, writing the placeholder, and calling the completion handler.

Important

Both the providePlaceholder(at:completionHandler:) and startProvidingItem(at:completionHandler:) methods can be triggered as other processes attempt to access documents provided by the File Provider extension. These methods may be called in response to user interaction with the document browser, or due to a coordinated read or coordinated write of the document’s URL.

Exactly which methods are triggered, and their sequence, depends on the type of coordinated access. For example, a coordinated read using the `NSFileCoordinatorReadingImmediatelyAvailableMetadataOnly` option triggers only the creation of a placeholder. As a result, your extension should not create dependencies between these methods. They may be called in any order.

### Look Up the Document’s File Provider Item

1.  Get the document’s persistent identifier by calling persistentIdentifierForItem(at:), and pass in the value of the `url` parameter.

2.  Call item(for:), and pass in the persistent identifier. This method returns the file provider item for the document.

### Write the Placeholder

1.  Get the placeholder URL by calling placeholderURL(for:), and pass in the value of the url parameter.

2.  Call writePlaceholder(at:withMetadata:), and pass in the placeholder URL and the file provider item.

### Call the Completion Handler

After writing the placeholder to disk, call the completion handler. If any errors occur, pass them to the completion handler. The system then passes the error back to the original coordinated read or write.

### Sample Implementation

```
override func providePlaceholder(at url: URL, completionHandler: @escaping (Error?) -> Void) {

    guard let identifier = persistentIdentifierForItem(at: url) else {
        completionHandler(NSFileProviderError(.noSuchItem))
        return
    }

    do {
        let fileProviderItem = try item(for: identifier)

        let placeholderURL = NSFileProviderManager.placeholderURL(for: url)
        try NSFileProviderManager.writePlaceholder(at: placeholderURL,
                                                   withMetadata: fileProviderItem)

        completionHandler(nil)
    }
    catch let error {
        completionHandler(error)
    }
}
```

## See Also

### Managing shared files

func itemChanged(at: URL)

Tells the File Provider extension that a document has changed.

func startProvidingItem(at: URL, completionHandler: ((any Error)?) -> Void)

Provides an actual file on disk for a placeholder.

func stopProvidingItem(at: URL)

Tells the File Provider extension that a given document is no longer being accessed.

