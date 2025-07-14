

- SwiftUI
- OpenImmersiveSpaceAction
-  callAsFunction(id:value:) 

Instance Method

# callAsFunction(id:value:)

Presents the immersive space that your app defines for the specified identifier and that handles the type of the presented value.

visionOS 1.0+

``` source
@discardableResult @MainActor
func callAsFunction(
    id: String,
    value: D
) async -> OpenImmersiveSpaceAction.Result where D : Decodable, D : Encodable, D : Hashable
```

## Parameters 

`id`  

The identifier of the immersive space to present.

`value`  

The value to present.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the openImmersiveSpace action with a string identifier and a value:

```
await openImmersiveSpace(id: "planet", value: planet.ID)
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction(id: String) async -> OpenImmersiveSpaceAction.Result

Presents an immersive space for the scene with the specified identifier.

func callAsFunction&lt;D>(value: D) async -> OpenImmersiveSpaceAction.Result

Presents the immersive space that handles the type of the presented value.

