

- AppKit
-  NSFilePromiseReceiver 

Class

# NSFilePromiseReceiver

An object that receives a file promise from the pasteboard.

macOS 10.12+

``` source
class NSFilePromiseReceiver
```

## Overview

Because NSFilePromiseReceiver implements the NSPasteboardReading protocol, you receive all file promises on the drag pasteboard as follows:

- Swift
- Objective-C

```
let filePromises = draggingPasteboard.readObjects(forClasses: [NSFilePromiseReceiver.self], options: nil)
```

```
NSArray filePromises = [draggingPasteboard readObjectsForClasses:@[[NSFilePromiseReceiver class]] options:nil];
```

Likewise, you can enumerate dragged items by calling the following:

- Swift
- Objective-C

```
draggingInfo.enumerateDraggingItems(options: [], for: view, classes: [NSFilePromiseReceiver.self], searchOptions: [:], using: {(draggingItem, idx, stop) in
    let filePromiseReceiver = draggingItem.item
    // Use filePromiseReceiver here for your task.
}
```

```
[draggingInfo enumerateDraggingItemsWithOptions:0 forView:view classes:@[[NSFilePromiseReceiver class]] searchOptions:@{} usingBlock:^(NSDraggingItem* draggingItem, NSInteger idx, BOOL* stop) {
    NSFilePromiseReceiver* filePromiseReceiver = draggingItem.item
    // Use filePromiseReceiver here for your task.
}];
```

Note

A non-item-based drag source may promise multiple files on the same pasteboard item. To be compatible with these drag sources, many NSFilePromiseReceiver methods return an array of values. Multiple-file item-based promises result in one NSFilePromiseReceiver per promised file.

## Topics

### Instance Properties

var fileNames: [String]

An array containing names of the promised files being written to the destination location.

var fileTypes: [String]

An array containing types of the promised files being written to the destination location.

### Instance Methods

func receivePromisedFiles(atDestination: URL, options: [AnyHashable : Any], operationQueue: OperationQueue, reader: (URL, (any Error)?) -> Void)

Fulfills the promises at the specified destination.

### Type Properties

class var readableDraggedTypes: [String]

An array containing dragged file types that are readable.

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
- NSPasteboardReading

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

protocol NSFilePromiseProviderDelegate

A set of methods that provides the name of the promised file and writes the file to the destination directory when the file promise is fulfilled.

