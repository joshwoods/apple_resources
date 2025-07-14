

- AppKit
- NSTextViewDelegate
-  undoManager(for:) 

Instance Method

# undoManager(for:)

Returns the undo manager for the specified text view.

macOS 10.0+

``` source
@MainActor
optional func undoManager(for view: NSTextView) -> UndoManager?
```

## Parameters 

`view`  

The text view whose undo manager should be returned.

## Return Value

The undo manager for `view`.

## Discussion

This method provides the flexibility to return a custom undo manager for the text view. Although `NSTextView` implements undo and redo for changes to text, applications may need a custom undo manager to handle interactions between changes to text and changes to other items in the application.

## See Also

### Related Documentation

Text System User Interface Layer Programming Guide

Cocoa Text Architecture Guide

