

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
- AnchoringComponent.Target.HandLocation
-  aboveHand 

Type Property

# aboveHand

An anchor location above the center of the palm in the world space, regardless how the hand is rotated.

Mac Catalyst 14.0+visionOS 1.0+

``` source
static let aboveHand: AnchoringComponent.Target.HandLocation
```

## Discussion

Content anchored this way has its positive y-axis pointing at the user’s head and its positive z-axis pointing towards the ground.

