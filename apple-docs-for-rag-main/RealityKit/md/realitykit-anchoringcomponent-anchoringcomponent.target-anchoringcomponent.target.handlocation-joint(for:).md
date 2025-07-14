

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
- AnchoringComponent.Target.HandLocation
-  joint(for:) 

Type Method

# joint(for:)

The function that returns the `HandLocation` based on `HandJoint`.

visionOS 2.0+

``` source
static func joint(for joint: AnchoringComponent.Target.HandLocation.HandJoint) -> AnchoringComponent.Target.HandLocation
```

## Parameters 

`joint`  

The joint to be targeted.

## Return Value

The `HandLocation` represents the hand joint.

