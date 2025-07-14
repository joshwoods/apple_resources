

- Foundation
- UndoManager
-  UndoManager.UserInfoKey 

Structure

# UndoManager.UserInfoKey

An extensible namespace for undo and redo user info keys.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct UserInfoKey
```

## Discussion

Extend this type with the names of user info keys you want to associate with undo actions, like this:

```
extension UndoManager.UserInfoKey {
    static let icon: UndoManager.UserInfoKey = "icon"
}
```

You then use this key when you set and get undo user info values.

```
self.undoManager.setActionUserInfoValue(Image(named: "new_layer"), forKey: .icon)

```

## Topics

### Creating a user info key from a raw value

init(String)

Creates a user info key from the given string.

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with user info

func setActionUserInfoValue(Any?, forKey: UndoManager.UserInfoKey)

Sets a user info value for an undo or redo action.

func undoActionUserInfoValue(forKey: UndoManager.UserInfoKey) -> Any?

Retrieves the undo action’s user info value for the given key.

func redoActionUserInfoValue(forKey: UndoManager.UserInfoKey) -> Any?

Retrieves the redo action’s user info value for the given key.

