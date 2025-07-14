

- SwiftUI
- DismissWindowAction
-  callAsFunction(value:) 

Instance Method

# callAsFunction(value:)

Dismisses the window defined by the window group that is presenting the specified value type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func callAsFunction(value: D) where D : Decodable, D : Encodable, D : Hashable
```

## Parameters 

`value`  

The value which is currently presented.

## Discussion

If multiple windows match the provided value, then they all will be dismissed. For dismissing a specific window in a specific group, use `dismissWindow(id:value:)`.

Don’t call this method directly. SwiftUI calls it when you call the dismissWindow action with an identifier and a value:

```
dismissWindow(value: message.id)
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction()

Dismisses the current window.

func callAsFunction(id: String)

Dismisses the window that’s associated with the specified identifier.

func callAsFunction&lt;D>(id: String, value: D)

Dismisses the window defined by the window group that is presenting the specified value type and that’s associated with the specified identifier.

