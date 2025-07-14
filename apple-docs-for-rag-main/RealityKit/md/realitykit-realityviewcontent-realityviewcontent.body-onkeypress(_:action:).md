

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  onKeyPress(\_:action:) 

Instance Method

# onKeyPress(\_:action:)

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS

``` source
nonisolated
func onKeyPress(
    _ key: KeyEquivalent,
    action: @escaping () -> KeyPress.Result
) -> some View
```

## Parameters 

`key`  

The key to match against incoming hardware keyboard events.

`action`  

The action to perform. Return `.handled` to consume the event and prevent further dispatch, or `.ignored` to allow dispatch to continue.

## Return Value

A modified view that binds hardware keyboard input when focused.

## Discussion

SwiftUI performs the action for key-down and key-repeat events.

