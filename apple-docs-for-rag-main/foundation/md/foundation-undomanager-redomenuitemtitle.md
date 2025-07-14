

- Foundation
- UndoManager
-  redoMenuItemTitle 

Instance Property

# redoMenuItemTitle

The title of the Redo menu command, such as Redo Paste.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var redoMenuItemTitle: String { get }
```

## Discussion

Returns “Redo” if no action name has been assigned or `nil` if there is nothing to redo.

## See Also

### Getting and localizing the menu item title

var undoMenuItemTitle: String

The title of the Undo menu command, such as Undo Paste.

func undoMenuTitle(forUndoActionName: String) -> String

Returns the localized title of the Undo menu command for the identified action.

func redoMenuTitle(forUndoActionName: String) -> String

Returns the localized title of the Redo menu command for the identified action.

