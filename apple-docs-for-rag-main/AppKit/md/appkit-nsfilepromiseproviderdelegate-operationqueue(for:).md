

- AppKit
- NSFilePromiseProviderDelegate
-  operationQueue(for:) 

Instance Method

# operationQueue(for:)

Returns the operation queue from which to issue the write request.

macOS 10.12+

``` source
@MainActor
optional func operationQueue(for filePromiseProvider: NSFilePromiseProvider) -> OperationQueue
```

## Parameters 

`filePromiseProvider`  

The file promise provider for the operation queue.

## Discussion

If this method isn’t implemented, the main operation queue is used. Although this method is optional, to avoid blocking your main thread, provide an operation queue other than the main operation queue.

## See Also

### Handling File Promises

func filePromiseProvider(NSFilePromiseProvider, fileNameForType: String) -> String

Provides the drag destination file’s name.

**Required**

func filePromiseProvider(NSFilePromiseProvider, writePromiseTo: URL, completionHandler: ((any Error)?) -> Void)

Writes the contents of a promise to the specified URL.

**Required**

