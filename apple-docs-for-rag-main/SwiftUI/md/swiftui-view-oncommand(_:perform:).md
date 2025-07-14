

- SwiftUI
- View
-  onCommand(\_:perform:) 

Instance Method

# onCommand(\_:perform:)

Adds an action to perform in response to the given selector.

macOS 10.15+

``` source
nonisolated
func onCommand(
    _ selector: Selector,
    perform action: (() -> Void)?
) -> some View
```

## Parameters 

`selector`  

The selector to register for `action`.

`action`  

The action to perform. If `action` is `nil`, `command` keeps its association with this view but doesn’t trigger.

## Return Value

A view that triggers `action` when the `command` occurs.

## Discussion

This view or one of the views it contains must be in focus in order for the action to trigger. Other actions for the same command on views *closer* to the view in focus take priority, potentially overriding this action.

## See Also

### Responding to commands

func onMoveCommand(perform: ((MoveCommandDirection) -> Void)?) -> some View

Adds an action to perform in response to a move command, like when the user presses an arrow key on a Mac keyboard, or taps the edge of the Siri Remote when controlling an Apple TV.

func onDeleteCommand(perform: (() -> Void)?) -> some View

Adds an action to perform in response to the system’s Delete command, or pressing either the ⌫ (backspace) or ⌦ (forward delete) keys while the view has focus.

func pageCommand&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V) -> some View

Steps a value through a range in response to page up or page down commands.

func onExitCommand(perform: (() -> Void)?) -> some View

Sets up an action that triggers in response to receiving the exit command while the view has focus.

func onPlayPauseCommand(perform: (() -> Void)?) -> some View

Adds an action to perform in response to the system’s Play/Pause command.

enum MoveCommandDirection

Specifies the direction of an arrow key movement.

