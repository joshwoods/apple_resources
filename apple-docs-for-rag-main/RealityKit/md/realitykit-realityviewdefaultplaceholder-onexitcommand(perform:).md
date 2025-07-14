

- RealityKit
- RealityViewDefaultPlaceholder
-  onExitCommand(perform:) 

Instance Method

# onExitCommand(perform:)

Sets up an action that triggers in response to receiving the exit command while the view has focus.

RealityKitSwiftUImacOS 10.15+tvOS 13.0+

``` source
nonisolated
func onExitCommand(perform action: (() -> Void)?) -> some View
```

## Discussion

The user generates an exit command by pressing the Menu button on tvOS, or the escape key on macOS.

