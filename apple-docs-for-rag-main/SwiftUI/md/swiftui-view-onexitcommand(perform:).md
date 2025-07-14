

- SwiftUI
- View
-  onExitCommand(perform:) 

Instance Method

# onExitCommand(perform:)

Sets up an action that triggers in response to receiving the exit command while the view has focus.

macOS 10.15+tvOS 13.0+

``` source
nonisolated
func onExitCommand(perform action: (() -> Void)?) -> some View
```

## Discussion

The user generates an exit command by pressing the Menu button on tvOS, or the escape key on macOS.

## See Also

### Responding to commands

func onMoveCommand(perform: ((MoveCommandDirection) -> Void)?) -> some View

Adds an action to perform in response to a move command, like when the user presses an arrow key on a Mac keyboard, or taps the edge of the Siri Remote when controlling an Apple TV.

func onDeleteCommand(perform: (() -> Void)?) -> some View

Adds an action to perform in response to the system’s Delete command, or pressing either the ⌫ (backspace) or ⌦ (forward delete) keys while the view has focus.

func pageCommand&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V) -> some View

Steps a value through a range in response to page up or page down commands.

func onPlayPauseCommand(perform: (() -> Void)?) -> some View

Adds an action to perform in response to the system’s Play/Pause command.

func onCommand(Selector, perform: (() -> Void)?) -> some View

Adds an action to perform in response to the given selector.

enum MoveCommandDirection

Specifies the direction of an arrow key movement.

