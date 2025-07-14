

- SwiftUI
- OpenWindowAction
-  callAsFunction(id:value:) 

Instance Method

# callAsFunction(id:value:)

Opens a window defined by the window group that presents the specified value type and that’s associated with the specified identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func callAsFunction(
    id: String,
    value: D
) where D : Decodable, D : Encodable, D : Hashable
```

## Parameters 

`id`  

The identifier of the scene to present.

`value`  

The value to present.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the openWindow action with an identifier and a value:

```
openWindow(id: "message", value: message.id)
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction(id: String)

Opens a window that’s associated with the specified identifier.

func callAsFunction&lt;D>(value: D)

Opens a window defined by a window group that presents the type of the specified value.

