

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  onKeyPress(phases:action:) 

Instance Method

# onKeyPress(phases:action:)

Performs an action if the user presses any key on a hardware keyboard while the view has focus.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS

``` source
nonisolated
func onKeyPress(
    phases: KeyPress.Phases = [.down, .repeat],
    action: @escaping (KeyPress) -> KeyPress.Result
) -> some View
```

## Parameters 

`phases`  

The key-press phases to match (`.down`, `.repeat`, and `.up`). The default value is `[.down, .repeat]`.

`action`  

The action to perform. The action receives a value describing the matched key event. Return `.handled` to consume the event and prevent further dispatch, or `.ignored` to allow dispatch to continue.

## Return Value

A modified view that binds hardware keyboard input when focused.

