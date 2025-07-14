

- SwiftUI
- OpenWindowAction
-  callAsFunction(value:) 

Instance Method

# callAsFunction(value:)

Opens a window defined by a window group that presents the type of the specified value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func callAsFunction(value: D) where D : Decodable, D : Encodable, D : Hashable
```

## Parameters 

`value`  

The value to present.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the openWindow action with a value:

```
openWindow(value: message.id)
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction(id: String)

Opens a window that’s associated with the specified identifier.

func callAsFunction&lt;D>(id: String, value: D)

Opens a window defined by the window group that presents the specified value type and that’s associated with the specified identifier.

