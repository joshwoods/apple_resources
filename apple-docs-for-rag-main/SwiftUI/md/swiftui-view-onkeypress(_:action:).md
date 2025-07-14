

- SwiftUI
- View
-  onKeyPress(\_:action:) 

Instance Method

# onKeyPress(\_:action:)

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

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

## See Also

### Responding to keyboard input

func onKeyPress(phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses any key on a hardware keyboard while the view has focus.

func onKeyPress(KeyEquivalent, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

func onKeyPress(characters: CharacterSet, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses one or more keys on a hardware keyboard while the view has focus.

func onKeyPress(keys: Set&lt;KeyEquivalent>, phases: KeyPress.Phases, action: (KeyPress) -> KeyPress.Result) -> some View

Performs an action if the user presses one or more keys on a hardware keyboard while the view has focus.

struct KeyPress

