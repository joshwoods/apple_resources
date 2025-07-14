

- SwiftUI
- PushWindowAction
-  callAsFunction(value:) 

Instance Method

# callAsFunction(value:)

Pushes a window defined by a window group that presents the type of the specified value.

visionOS 2.0+

``` source
@MainActor
func callAsFunction(value: D) where D : Decodable, D : Encodable, D : Hashable
```

## Parameters 

`value`  

The value to present.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the pushWindow action with a value:

```
pushWindow(value: video.id)
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

