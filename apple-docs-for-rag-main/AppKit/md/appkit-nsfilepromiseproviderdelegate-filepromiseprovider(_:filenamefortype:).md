

- AppKit
- NSFilePromiseProviderDelegate
-  filePromiseProvider(\_:fileNameForType:) 

Instance Method

# filePromiseProvider(\_:fileNameForType:)

Provides the drag destination file’s name.

macOS 10.12+

``` source
@MainActor
func filePromiseProvider(
    _ filePromiseProvider: NSFilePromiseProvider,
    fileNameForType fileType: String
) -> String
```

**Required**

## Parameters 

`filePromiseProvider`  

The file promise provider.

`fileType`  

A string describing the type of file being provided.

## Discussion

This method is called when the drag destination fulfills the file promise. Determine and return the final filename (a base filename, not a full path).

Note

Don’t start writing the file to the destination directory until the drag process is complete. The drag process stops to wait for the method to return, and if it has to wait too long, the drag could be canceled.

## See Also

### Handling File Promises

func filePromiseProvider(NSFilePromiseProvider, writePromiseTo: URL, completionHandler: ((any Error)?) -> Void)

Writes the contents of a promise to the specified URL.

**Required**

func operationQueue(for: NSFilePromiseProvider) -> OperationQueue

Returns the operation queue from which to issue the write request.

