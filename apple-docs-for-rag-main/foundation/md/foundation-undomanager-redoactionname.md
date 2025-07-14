

- Foundation
- UndoManager
-  redoActionName 

Instance Property

# redoActionName

The name identifying the redo action.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var redoActionName: String { get }
```

## Discussion

The redo action name. Returns an empty string (`@""`) if no action name has been assigned or if there is nothing to redo.

For example, if the menu title is “Redo Delete,” the string returned is “Delete.”

## See Also

### Managing the action name

var undoActionName: String

The name identifying the undo action.

func setActionName(String)

Sets the name of the action associated with the Undo or Redo command.

