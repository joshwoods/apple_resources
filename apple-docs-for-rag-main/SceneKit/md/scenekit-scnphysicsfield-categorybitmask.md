

- SceneKit
- SCNPhysicsField
-  categoryBitMask 

Instance Property

# categoryBitMask

A mask that defines which categories this physics field belongs to.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var categoryBitMask: Int { get set }
```

## Discussion

To determine whether a field affects a physics body, SceneKit performs a bitwise AND operation on the field’s category bit mask and the body’s categoryBitMask property. If the result is a nonzero value, SceneKit computes and applies the force of the field on the body. To determine whether a field affects the particles spawned by an SCNParticleSystem object, SceneKit performs the same check using the categoryBitMask property of the node containing the particle system.

Use this property to create fields which affect only certain bodies in your scene. Reducing the number of bodies affected by fields can also improve simulation performance.

