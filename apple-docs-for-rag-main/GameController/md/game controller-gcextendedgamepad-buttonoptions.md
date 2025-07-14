

- Game Controller
- GCExtendedGamepad
-  buttonOptions 

Instance Property

# buttonOptions

The controller’s secondary menu button element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var buttonOptions: GCControllerButtonInput? { get }
```

## Discussion

You can use the secondary menu to configure graphics and sound, and to pause the game.

## See Also

### Getting face button inputs

var buttonMenu: GCControllerButtonInput

The primary menu button element that players use to enter the main menu and pause the game.

var buttonHome: GCControllerButtonInput?

The main menu button element that players use to enter the secondary menu and pause the game.

var buttonA: GCControllerButtonInput

The bottom face button that uses *A* or another indicator as its label.

var buttonB: GCControllerButtonInput

The right face button that uses *B* or another indicator as its label.

var buttonX: GCControllerButtonInput

The left face button that uses *X* or another indicator as its label.

var buttonY: GCControllerButtonInput

The top face button that uses *Y* or another indicator as its label.

