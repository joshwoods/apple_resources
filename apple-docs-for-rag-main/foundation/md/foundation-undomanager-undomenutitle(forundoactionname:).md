

- Foundation
- UndoManager
-  undoMenuTitle(forUndoActionName:) 

Instance Method

# undoMenuTitle(forUndoActionName:)

Returns the localized title of the Undo menu command for the identified action.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func undoMenuTitle(forUndoActionName actionName: String) -> String
```

## Parameters 

`actionName`  

The name of the undo action.

## Return Value

The localized title of the undo menu item.

## Discussion

Override this method if you want to customize the localization behavior. This method is invoked by undoMenuItemTitle.

## See Also

### Getting and localizing the menu item title

var undoMenuItemTitle: String

The title of the Undo menu command, such as Undo Paste.

var redoMenuItemTitle: String

The title of the Redo menu command, such as Redo Paste.

func redoMenuTitle(forUndoActionName: String) -> String

Returns the localized title of the Redo menu command for the identified action.

