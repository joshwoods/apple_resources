

- SwiftUI
- View
-  onKeyPress(phases:action:) 

Instance Method

# onKeyPress(phases:action:)

Performs an action if the user presses any key on a hardware keyboard while the view has focus.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

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

## See Also

### Responding to keyboard input

func onKeyPress(KeyEquivalent, action: () -> KeyPress.Result) -> some View

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

func onKeyPress(KeyEquivalent, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

func onKeyPress(characters: CharacterSet, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses one or more keys on a hardware keyboard while the view has focus.

func onKeyPress(keys: Set&lt;KeyEquivalent>, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses one or more keys on a hardware keyboard while the view has focus.

struct KeyPress

