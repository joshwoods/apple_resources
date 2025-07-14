

- AppKit
-  NSFilePromiseProviderDelegate 

Protocol

# NSFilePromiseProviderDelegate

A set of methods that provides the name of the promised file and writes the file to the destination directory when the file promise is fulfilled.

macOS

``` source
protocol NSFilePromiseProviderDelegate : NSObjectProtocol
```

## Topics

### Handling File Promises

func filePromiseProvider(NSFilePromiseProvider, fileNameForType: String) -> String

Provides the drag destination file’s name.

**Required**

func filePromiseProvider(NSFilePromiseProvider, writePromiseTo: URL, completionHandler: ((any Error)?) -> Void)

Writes the contents of a promise to the specified URL.

**Required**

func operationQueue(for: NSFilePromiseProvider) -> OperationQueue

Returns the operation queue from which to issue the write request.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### File Promises

Supporting Drag and Drop Through File Promises

Receive and provide file promises to support dragged app files and pasteboard operations.

Supporting Table View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

Supporting Collection View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

class NSFilePromiseProvider

An object that provides a promise for the pasteboard.

class NSFilePromiseReceiver

An object that receives a file promise from the pasteboard.

