

- Foundation
- UndoManager
-  setActionName(\_:) 

Instance Method

# setActionName(\_:)

Sets the name of the action associated with the Undo or Redo command.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setActionName(_ actionName: String)
```

## Parameters 

`actionName`  

The name of the action.

## Discussion

If `actionName` is an empty string, the action name currently associated with the menu command is removed. There is no effect if `actionName` is `nil`.

## See Also

### Managing the action name

var undoActionName: String

The name identifying the undo action.

var redoActionName: String

The name identifying the redo action.

