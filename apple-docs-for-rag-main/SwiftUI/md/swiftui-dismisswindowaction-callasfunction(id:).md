

- SwiftUI
- DismissWindowAction
-  callAsFunction(id:) 

Instance Method

# callAsFunction(id:)

Dismisses the window that’s associated with the specified identifier.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func callAsFunction(id: String)
```

## Parameters 

`id`  

The identifier of the scene to dismiss.

## Discussion

When the specified identifier represents a WindowGroup, all of the open windows in that group will be dismissed. For dismissing a single window associated to a `WindowGroup` scene, use `dismissWindow(value:)` or `dismissWindow(id:value:)`.

Don’t call this method directly. SwiftUI calls it when you call the dismissWindow action with an identifier:

```
dismissWindow(id: "message")
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction()

Dismisses the current window.

func callAsFunction&lt;D>(id: String, value: D)

Dismisses the window defined by the window group that is presenting the specified value type and that’s associated with the specified identifier.

func callAsFunction&lt;D>(value: D)

Dismisses the window defined by the window group that is presenting the specified value type.

