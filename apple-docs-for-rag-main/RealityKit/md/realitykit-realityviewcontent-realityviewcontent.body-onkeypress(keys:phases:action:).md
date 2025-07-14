

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  onKeyPress(keys:phases:action:) 

Instance Method

# onKeyPress(keys:phases:action:)

Performs an action if the user presses one or more keys on a hardware keyboard while the view has focus.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS

``` source
nonisolated
func onKeyPress(
    keys: Set,
    phases: KeyPress.Phases = [.down, .repeat],
    action: @escaping (KeyPress) -> KeyPress.Result
) -> some View
```

## Parameters 

`keys`  

A set of keys to match against incoming hardware keyboard events.

`phases`  

The key-press phases to match (`.down`, `.repeat`, and `.up`). The default value is `[.down, .repeat]`.

`action`  

The action to perform. The action receives a value describing the matched key event. Return `.handled` to consume the event and prevent further dispatch, or `.ignored` to allow dispatch to continue.

## Return Value

A modified view that binds keyboard input when focused.

