

- SwiftUI
- DismissWindowAction
-  callAsFunction(id:value:) 

Instance Method

# callAsFunction(id:value:)

Dismisses the window defined by the window group that is presenting the specified value type and that’s associated with the specified identifier.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func callAsFunction(
    id: String,
    value: D
) where D : Decodable, D : Encodable, D : Hashable
```

## Parameters 

`id`  

The identifier of the scene to dismiss.

`value`  

The value which is currently presented.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the dismissWindow action with an identifier and a value:

```
dismissWindow(id: "message", value: message.id)
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction()

Dismisses the current window.

func callAsFunction(id: String)

Dismisses the window that’s associated with the specified identifier.

func callAsFunction&lt;D>(value: D)

Dismisses the window defined by the window group that is presenting the specified value type.

