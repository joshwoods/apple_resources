

- SpriteKit
-  SKTransition 

Class

# SKTransition

An object used to perform an animated transition to a new scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKTransition
```

## Overview

Scenes are the basic building blocks of games. Typically, you design self-contained scenes for the parts of your game, and then transition between these scenes as necessary. For example, you might create different scene classes to represent any or all of the following concepts:

- A loading scene to display while other content is loaded

- A main menu scene to choose what kind of game the user wants to play

- A scene to configure the details of the specific kind of game the user chose

- A scene that provides the gameplay

- A scene displayed when gameplay ends

When you present a new scene in a view that is already presenting a scene, you have the option of using a transition to animate the change from the old scene to the new scene. Using a transition provides continuity so that the scene change is not quite so abrupt.

## Topics

### Creating Transitions

Transitioning Between Two Scenes

Configuring Whether Animations Play During the Transition

class func crossFade(withDuration: TimeInterval) -> SKTransition

Creates a cross fade transition.

class func doorsCloseHorizontal(withDuration: TimeInterval) -> SKTransition

Creates a transition where the new scene appears as a pair of closing horizontal doors.

class func doorsCloseVertical(withDuration: TimeInterval) -> SKTransition

Creates a transition where the new scene appears as a pair of closing vertical doors.

class func doorsOpenHorizontal(withDuration: TimeInterval) -> SKTransition

Creates a transition where the new scene appears as a pair of opening horizontal doors.

class func doorsOpenVertical(withDuration: TimeInterval) -> SKTransition

Creates a transition where the new scene appears as a pair of opening vertical doors.

class func doorway(withDuration: TimeInterval) -> SKTransition

Creates a transition where the previous scene disappears as a pair of opening doors.

class func fade(with: UIColor, duration: TimeInterval) -> SKTransition

Creates a transition that first fades to a constant color and then fades to the new scene.

class func fade(withDuration: TimeInterval) -> SKTransition

Creates a transition that first fades to black and then fades to the new scene.

class func flipHorizontal(withDuration: TimeInterval) -> SKTransition

Creates a transition where the two scenes are flipped across a horizontal line running through the center of the view.

class func flipVertical(withDuration: TimeInterval) -> SKTransition

Creates a transition where the two scenes are flipped across a vertical line running through the center of the view.

class func moveIn(with: SKTransitionDirection, duration: TimeInterval) -> SKTransition

Creates a transition where the new scene moves in on top of the old scene.

class func push(with: SKTransitionDirection, duration: TimeInterval) -> SKTransition

Creates a transition where the new scene moves in, pushing the old scene out of the view.

class func reveal(with: SKTransitionDirection, duration: TimeInterval) -> SKTransition

Creates a transition where the old scene moves out of the view, revealing the new scene underneath it.

init(ciFilter: CIFilter, duration: TimeInterval)

Creates a transition that uses a Core Image filter to perform the transition.

### Pausing

var pausesIncomingScene: Bool

A Boolean value that determines whether the incoming scene is paused during the transition.

var pausesOutgoingScene: Bool

A Boolean value that determines whether the outgoing scene is paused during the transition.

### Constants

enum SKTransitionDirection

For some transitions, the direction in which the transition is performed.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Displaying a Scene

var scene: SKScene?

The scene currently presented by this view.

func presentScene(SKScene?)

Presents a scene.

func presentScene(SKScene, transition: SKTransition)

Transitions from the current scene to a new scene.

