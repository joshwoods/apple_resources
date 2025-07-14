

- UIKit
- UIScene
-  pointerLockState 

Instance Property

# pointerLockState

The pointer lock state for the scene.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var pointerLockState: UIPointerLockState? { get }
```

## Discussion

If a scene can’t lock the pointer, this property is `nil`.

## See Also

### Getting the pointer lock state

class UIPointerLockState

An object that contains information about a scene’s pointer lock state.

