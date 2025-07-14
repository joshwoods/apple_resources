

- AppKit
-  NSFilePromiseProvider 

Class

# NSFilePromiseProvider

An object that provides a promise for the pasteboard.

macOS 10.12+

``` source
class NSFilePromiseProvider
```

## Overview

A file promise is a possible future file of a specified type. When you’re working with drag and drop, use promises to indicate intent for future action. Avoid loading or performing any actions on the file until the promise completes.

Use the NSFilePromiseProvider class when creating file promises. Instantiate one NSFilePromiseProvider for each file promised. Set the fileType and delegate properties before writing any NSFilePromiseProvider to the pasteboard. The file type must be a Uniform Type Identifier (UTI) that ultimately conforms to `kUTTypeData` or `kUTTypeDirectory`. The NSFilePromiseProviderDelegate will write the promised file to the destination directory.

Optionally, you may attach a `userInfo` object of your choosing to the NSFilePromiseProvider to determine which promise is being referenced when promising multiple files under the same NSFilePromiseProviderDelegate instance.

## Topics

### Initializers

init()

Initializes a file promise provider.

convenience init(fileType: String, delegate: any NSFilePromiseProviderDelegate)

Initializes a file promise provider for a certain file type.

### Instance Properties

var delegate: (any NSFilePromiseProviderDelegate)?

var fileType: String

The file type of the file promise provider.

var userInfo: Any?

Optional user information to pass to the file promise provider.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- NSPasteboardWriting

## See Also

### File Promises

Supporting Drag and Drop Through File Promises

Receive and provide file promises to support dragged app files and pasteboard operations.

Supporting Table View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

Supporting Collection View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

protocol NSFilePromiseProviderDelegate

A set of methods that provides the name of the promised file and writes the file to the destination directory when the file promise is fulfilled.

class NSFilePromiseReceiver

An object that receives a file promise from the pasteboard.

