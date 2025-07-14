

- SceneKit
- SCNPhysicsField
-  customField(evaluationBlock:) 

Type Method

# customField(evaluationBlock:)

Creates a field that runs the specified block to determine the force a field applies to each object in its area of effect.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func customField(evaluationBlock block: @escaping SCNFieldForceEvaluator) -> SCNPhysicsField
```

## Parameters 

`block`  

A block that SceneKit runs for each object in the field’s area of effect. See SCNFieldForceEvaluator.

## Return Value

A physics field object. To use the field in a scene, attach it to the physicsField property of an SCNNode object.

## Discussion

For custom physics fields, SceneKit ignores the direction, strength, falloffExponent, and minimumDistance properties. Instead, SceneKit calls your block to determine the direction and magnitude of force to apply to each physics body or particle in the field’s area of effect.

