

- Foundation
- UndoManager
-  undoActionName 

Instance Property

# undoActionName

The name identifying the undo action.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var undoActionName: String { get }
```

## Discussion

The undo action name. Returns an empty string (`@""`) if no action name has been assigned or if there is nothing to undo.

For example, if the menu title is “Undo Delete,” the string returned is “Delete.”

## See Also

### Managing the action name

var redoActionName: String

The name identifying the redo action.

func setActionName(String)

Sets the name of the action associated with the Undo or Redo command.

