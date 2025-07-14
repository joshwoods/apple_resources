

- AppKit
- NSResponder
-  undoManager 

Instance Property

# undoManager

The undo manager for this responder.

macOS

``` source
@MainActor
var undoManager: UndoManager? { get }
```

## Discussion

The `NSResponder` implementation simply invokes this property on the next responder.

