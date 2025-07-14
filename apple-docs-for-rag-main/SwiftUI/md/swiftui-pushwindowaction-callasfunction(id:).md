

- SwiftUI
- PushWindowAction
-  callAsFunction(id:) 

Instance Method

# callAsFunction(id:)

Pushes a window that is associated with the specified identifier.

visionOS 2.0+

``` source
@MainActor
func callAsFunction(id: String)
```

## Parameters 

`id`  

The identifier of the scene to present.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the pushWindow action with an identifier:

```
pushWindow(id: "viewer")
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

