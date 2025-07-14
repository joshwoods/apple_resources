

- SpriteKit
- SKTransition
-  reveal(with:duration:) 

Type Method

# reveal(with:duration:)

Creates a transition where the old scene moves out of the view, revealing the new scene underneath it.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func reveal(
    with direction: SKTransitionDirection,
    duration sec: TimeInterval
) -> SKTransition
```

## Parameters 

`direction`  

The direction of the reveal. Possible values are described in SKTransitionDirection.

`sec`  

The duration of the transition.

## Return Value

A new transition.

## See Also

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

init(ciFilter: CIFilter, duration: TimeInterval)

Creates a transition that uses a Core Image filter to perform the transition.

