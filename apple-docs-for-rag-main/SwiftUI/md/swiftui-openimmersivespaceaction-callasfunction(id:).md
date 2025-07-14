

- SwiftUI
- OpenImmersiveSpaceAction
-  callAsFunction(id:) 

Instance Method

# callAsFunction(id:)

Presents an immersive space for the scene with the specified identifier.

visionOS 1.0+

``` source
@discardableResult @MainActor
func callAsFunction(id: String) async -> OpenImmersiveSpaceAction.Result
```

## Parameters 

`id`  

The identifier of the immersive space to present.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the openImmersiveSpace action with a string identifier:

```
await openImmersiveSpace(id: "planet")
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction&lt;D>(id: String, value: D) async -> OpenImmersiveSpaceAction.Result

Presents the immersive space that your app defines for the specified identifier and that handles the type of the presented value.

func callAsFunction&lt;D>(value: D) async -> OpenImmersiveSpaceAction.Result

Presents the immersive space that handles the type of the presented value.

