

- SpriteKit
- SKTransition
-  fade(with:duration:) 

Type Method

# fade(with:duration:)

Creates a transition that first fades to a constant color and then fades to the new scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
class func fade(
    with color: NSColor,
    duration sec: TimeInterval
) -> SKTransition
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
class func fade(
    with color: UIColor,
    duration sec: TimeInterval
) -> SKTransition
```

## Parameters 

`color`  

The color to use as the fade color.

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

