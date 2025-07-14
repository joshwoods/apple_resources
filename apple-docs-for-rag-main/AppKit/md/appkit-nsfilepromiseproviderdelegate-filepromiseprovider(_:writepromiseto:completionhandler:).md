

- AppKit
- NSFilePromiseProviderDelegate
-  filePromiseProvider(\_:writePromiseTo:completionHandler:) 

Instance Method

# filePromiseProvider(\_:writePromiseTo:completionHandler:)

Writes the contents of a promise to the specified URL.

macOS 10.12+

``` source
nonisolated
func filePromiseProvider(
    _ filePromiseProvider: NSFilePromiseProvider,
    writePromiseTo url: URL,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
nonisolated
func filePromiseProvider(
    _ filePromiseProvider: NSFilePromiseProvider,
    writePromiseTo url: URL
) async throws
```

**Required**

## Parameters 

`filePromiseProvider`  

The file promise provider.

`url`  

The destination URL to write to.

`completionHandler`  

A completion handler to execute after the file has been written.

## Discussion

This method is called after the drag is complete. The request executes on the OperationQueue supplied by operationQueue(for:).

Call the completion handler with the file contents wrapped in NSFileCoordinator. Be sure to write your file to the input `url` parameter.

## See Also

### Handling File Promises

func filePromiseProvider(NSFilePromiseProvider, fileNameForType: String) -> String

Provides the drag destination file’s name.

**Required**

func operationQueue(for: NSFilePromiseProvider) -> OperationQueue

Returns the operation queue from which to issue the write request.

