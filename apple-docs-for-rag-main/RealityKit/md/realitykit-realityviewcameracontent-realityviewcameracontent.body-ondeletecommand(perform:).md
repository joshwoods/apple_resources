

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  onDeleteCommand(perform:) 

Instance Method

# onDeleteCommand(perform:)

Adds an action to perform in response to the system’s Delete command, or pressing either the ⌫ (backspace) or ⌦ (forward delete) keys while the view has focus.

RealityKitSwiftUImacOS 10.15+

``` source
nonisolated
func onDeleteCommand(perform action: (() -> Void)?) -> some View
```

