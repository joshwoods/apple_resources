

- AppKit
-  NSTextStorageObserving 

Protocol

# NSTextStorageObserving

Optional methods that delegates implement to handle editing and transaction processing.

macOS 12.0+

``` source
protocol NSTextStorageObserving : NSObjectProtocol
```

## Topics

### Accessing the text storage

var textStorage: NSTextStorage?

**Required**

### Managing the editing process

func performEditingTransaction(for: NSTextStorage, using: () -> Void)

**Required**

func processEditing(for: NSTextStorage, edited: NSTextStorageEditActions, range: NSRange, changeInLength: Int, invalidatedRange: NSRange)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTextContentStorage

## See Also

### Accessing the storage controller

var textStorageObserver: (any NSTextStorageObserving)?

The observer for the text storage object.

