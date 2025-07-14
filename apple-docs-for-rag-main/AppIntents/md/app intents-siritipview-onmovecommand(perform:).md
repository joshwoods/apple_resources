

- App Intents
- SiriTipView
-  onMoveCommand(perform:) 

Instance Method

# onMoveCommand(perform:)

Adds an action to perform in response to a move command, like when the user presses an arrow key on a Mac keyboard, or taps the edge of the Siri Remote when controlling an Apple TV.

AppIntentsSwiftUImacOS 10.15+tvOS 13.0+

``` source
nonisolated
func onMoveCommand(perform action: ((MoveCommandDirection) -> Void)?) -> some View
```

