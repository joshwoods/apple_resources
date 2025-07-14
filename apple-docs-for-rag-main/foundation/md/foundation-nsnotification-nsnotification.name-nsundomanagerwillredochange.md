

- Foundation
- NSNotification
- NSNotification.Name
-  NSUndoManagerWillRedoChange 

Type Property

# NSUndoManagerWillRedoChange

Posted just before an undo manager performs a redo operation.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSUndoManagerWillRedoChange: NSNotification.Name
```

## Discussion

The notification object is the UndoManager object. This notification doesn’t contain a `userInfo` dictionary.

The system posts this notification on the actor, thread, or dispatch queue that calls redo().

## See Also

### Working with notifications

static let NSUndoManagerCheckpoint: NSNotification.Name

Posted whenever an undo manager opens or closes an undo group (except when it opens a top-level group) and when checking the redo stack.

static let NSUndoManagerDidOpenUndoGroup: NSNotification.Name

Posted whenever an undo manager opens an undo group.

static let NSUndoManagerDidRedoChange: NSNotification.Name

Posted just after an undo manager performs a redo operation.

static let NSUndoManagerDidUndoChange: NSNotification.Name

Posted just after an undo manager performs an undo operation.

static let NSUndoManagerWillCloseUndoGroup: NSNotification.Name

Posted before an undo manager closes an undo group.

static let NSUndoManagerDidCloseUndoGroup: NSNotification.Name

Posted after an undo manager closes an undo group.

static let NSUndoManagerWillUndoChange: NSNotification.Name

Posted just before an undo manager performs an undo operation.

let NSUndoManagerGroupIsDiscardableKey: String

A key, used in a notification’s user info, that indicates the undo group contains only discardable actions.

