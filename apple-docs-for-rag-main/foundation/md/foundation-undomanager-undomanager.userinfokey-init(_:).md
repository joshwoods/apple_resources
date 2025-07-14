

- Foundation
- UndoManager
- UndoManager.UserInfoKey
-  init(\_:) 

Initializer

# init(\_:)

Creates a user info key from the given string.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(_ rawValue: String)
```

## Parameters 

`rawValue`  

The raw value string.

## Discussion

Don’t use this initializer. Instead, extend the UndoManager.UserInfoKey namespace as follows:

```
extension UndoManager.UserInfoKey {
    static let icon: UndoManager.UserInfoKey = "icon"
}
```

## See Also

### Creating a user info key from a raw value

init(rawValue: String)

