

- AppKit
- NSDocument
- NSDocument.ChangeType
-  NSDocument.ChangeType.changeCleared 

Case

# NSDocument.ChangeType.changeCleared

Set change count to 0. The document has been synchronized with its file or file package. For example, saveToURL:ofType:forSaveOperation:error: passes this value for a successful NSDocument.SaveOperationType.saveOperation or NSDocument.SaveOperationType.saveAsOperation. The revertToSaved(_:) method does too.

macOS

``` source
case changeCleared
```

## See Also

### Constants

case changeDone

Increment change count. Pass this value to the updateChangeCount(_:) method to indicate that a single change has been done. For example, the built-in undo support in the NSDocument class passes this value whenever a document receives an NSUndoManagerDidCloseUndoGroup notification from its own undo manager.

case changeUndone

Decrement change count. A single change has been undone. For example, the built-in undo support of `NSDocument` passes this value whenever a document receives an NSUndoManagerDidUndoChange from its own undo manager.

case changeReadOtherContents

The document has been initialized with the contents of a file or file package other than the one whose location is in the fileURL property, and therefore can’t possibly be synchronized with its persistent representation. For example, init(for:withContentsOf:ofType:) passes this value when the two passed-in URLs are not equal to indicate that an autosaved document is being reopened.

case changeAutosaved

The document’s contents have been autosaved. For example, saveToURL:ofType:forSaveOperation:error: passes this value for a successful NSAutosaveOperation.

case changeRedone

A single change has been redone. For example, the built-in undo support of `NSDocument` passes this value whenever a document receives an NSUndoManagerDidRedoChange from its own undo manager.

case changeDiscardable

