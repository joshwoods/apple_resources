

- Foundation
- UndoManager
-  redoActionUserInfoValue(forKey:) 

Instance Method

# redoActionUserInfoValue(forKey:)

Retrieves the redo action’s user info value for the given key.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func redoActionUserInfoValue(forKey key: UndoManager.UserInfoKey) -> Any?
```

## Parameters 

`key`  

The key associated with the value to return.

## Return Value

The value that you previously registered to this key with setActionUserInfoValue(_:forKey:), or `nil` if the key is absent.

## Discussion

Use this method to retrieve a user info value for the redo action you previously set with setActionUserInfoValue(_:forKey:).

In this example, an app’s `redoButton()` method provides a SwiftUI view that incorporates a previously assigned icon for the action:

```
func redoButton() -> some SwiftUI.View {
    Button(action: {
        self.undoManager.redo()
    }) {
        Label(self.undoManager.redoActionName,
              image: self.undoManager.redoActionUserInfoValue(forKey: .icon) as? Image)
    }
}
```

## See Also

### Working with user info

func setActionUserInfoValue(Any?, forKey: UndoManager.UserInfoKey)

Sets a user info value for an undo or redo action.

func undoActionUserInfoValue(forKey: UndoManager.UserInfoKey) -> Any?

Retrieves the undo action’s user info value for the given key.

struct UserInfoKey

An extensible namespace for undo and redo user info keys.

