

- Game Controller
- GCExtendedGamepad
-  buttonHome 

Instance Property

# buttonHome

The main menu button element that players use to enter the secondary menu and pause the game.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var buttonHome: GCControllerButtonInput? { get }
```

## Discussion

If the system doesn’t process the main menu events, it passes the events to your app.

## See Also

### Getting face button inputs

var buttonMenu: GCControllerButtonInput

The primary menu button element that players use to enter the main menu and pause the game.

var buttonOptions: GCControllerButtonInput?

The controller’s secondary menu button element.

var buttonA: GCControllerButtonInput

The bottom face button that uses *A* or another indicator as its label.

var buttonB: GCControllerButtonInput

The right face button that uses *B* or another indicator as its label.

var buttonX: GCControllerButtonInput

The left face button that uses *X* or another indicator as its label.

var buttonY: GCControllerButtonInput

The top face button that uses *Y* or another indicator as its label.

