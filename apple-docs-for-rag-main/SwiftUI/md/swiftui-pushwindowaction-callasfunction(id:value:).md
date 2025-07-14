

- SwiftUI
- PushWindowAction
-  callAsFunction(id:value:) 

Instance Method

# callAsFunction(id:value:)

Pushes a window defined by the window group that presents the specified value type and that is associated with the specified identifier.

visionOS 2.0+

``` source
@MainActor
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

Don’t call this method directly. SwiftUI calls it when you call the pushWindow action with an identifier and a value:

```
pushWindow(id: "viewer", value: video.id)
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

