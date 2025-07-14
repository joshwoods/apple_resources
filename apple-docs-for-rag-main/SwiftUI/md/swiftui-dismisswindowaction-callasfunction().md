

- SwiftUI
- DismissWindowAction
-  callAsFunction() 

Instance Method

# callAsFunction()

Dismisses the current window.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func callAsFunction()
```

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the dismissWindow action:

```
dismissWindow()
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction(id: String)

Dismisses the window that’s associated with the specified identifier.

func callAsFunction&lt;D>(id: String, value: D)

Dismisses the window defined by the window group that is presenting the specified value type and that’s associated with the specified identifier.

func callAsFunction&lt;D>(value: D)

Dismisses the window defined by the window group that is presenting the specified value type.

