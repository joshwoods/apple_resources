

- SwiftUI
- View
-  handlesGameControllerEvents(matching:) 

Instance Method

# handlesGameControllerEvents(matching:)

Specifies the game controllers events which should be delivered through the GameController framework when the view, or one of its descendants has focus.

GameControllerSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
nonisolated
func handlesGameControllerEvents(matching types: GCUIEventTypes) -> some View
```

## Discussion

```
SpriteView(scene: MyGameScene())
.handlesGameControllerEvents(matching: .gamepad)
.focused(true)
```

