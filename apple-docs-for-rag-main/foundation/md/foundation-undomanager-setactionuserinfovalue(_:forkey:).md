

- Foundation
- UndoManager
-  setActionUserInfoValue(\_:forKey:) 

Instance Method

# setActionUserInfoValue(\_:forKey:)

Sets a user info value for an undo or redo action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func setActionUserInfoValue(
    _ info: Any?,
    forKey key: UndoManager.UserInfoKey
)
```

## Parameters 

`info`  

The value to save in the action’s user info.

`key`  

The key to associate with the user info value.

## Discussion

Set user info on an undo action to provide custom information to the action beyond its action name. You can use this for things like an icon to represent the undoable action, or a timestamp of when the undo manager registers the action.

Start by extending UndoManager.UserInfoKey with key names to identify the user info values you want to associate with undo actions.

```
extension UndoManager.UserInfoKey {
    static let icon: UndoManager.UserInfoKey = "icon"
}
```

Then set the user info value with this key as part of registering the undoable action. In this example, an app’s `insertLayer()` method provides a custom icon before setting up an undo action that calls the app’s `removeLayer()` method:

```
func insertLayer() {
    self.undoManager.setActionName("Insert layer")
    self.undoManager.setActionUserInfoValue(Image(named: "new_layer"), forKey: .icon)

    self.layers.append(Layer())

    self.undoManager.registerUndo(withTarget: self) {
        $0.removeLayer()
    }
}
```

## See Also

### Working with user info

func undoActionUserInfoValue(forKey: UndoManager.UserInfoKey) -> Any?

Retrieves the undo action’s user info value for the given key.

func redoActionUserInfoValue(forKey: UndoManager.UserInfoKey) -> Any?

Retrieves the redo action’s user info value for the given key.

struct UserInfoKey

An extensible namespace for undo and redo user info keys.

