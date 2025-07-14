

- RealityKit
- GroundingShadowComponent
- GroundingShadowComponent.FadeBehaviorNearPhysicalObjects
-  GroundingShadowComponent.FadeBehaviorNearPhysicalObjects.default 

Case

# GroundingShadowComponent.FadeBehaviorNearPhysicalObjects.default

The default grounding shadow behavior for the device’s platform.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
case `default`
```

## Discussion

In visionOS, the default case is equivalent to GroundingShadowComponent.FadeBehaviorNearPhysicalObjects.fade when the the system can detect the entity represents a UI; otherwise,GroundingShadowComponent.FadeBehaviorNearPhysicalObjects.constant.

In iOS, the default case is equivalent to GroundingShadowComponent.FadeBehaviorNearPhysicalObjects.constant.

