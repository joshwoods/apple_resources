

- AppKit
-  NSTextStorageDelegate 

Protocol

# NSTextStorageDelegate

The optional methods that delegates of text storage objects implement to handle text-edit processing.

macOS

``` source
protocol NSTextStorageDelegate : NSObjectProtocol
```

## Topics

### Processing edit actions

func textStorage(NSTextStorage, willProcessEditing: NSTextStorageEditActions, range: NSRange, changeInLength: Int)

The method the framework calls when a text storage object is about to process edits.

func textStorage(NSTextStorage, didProcessEditing: NSTextStorageEditActions, range: NSRange, changeInLength: Int)

The method the framework calls when a text storage object has finished processing edits.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Processing the editing actions

var delegate: (any NSTextStorageDelegate)?

The delegate for the text storage object.

