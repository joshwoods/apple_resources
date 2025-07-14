

- SpriteKit
- SKEmitterNode
-  fieldBitMask 

Instance Property

# fieldBitMask

A mask that defines which categories of physics fields can exert forces on the particles.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var fieldBitMask: UInt32 { get set }
```

**watchOS**

``` source
var fieldBitMask: UInt32 { get set }
```

## Discussion

When a particle is inside the region of a SKFieldNode object, that field node’s categoryBitMask property is compared to the emitter’s fieldBitMask property by performing a logical AND operation. If the result is a non-zero value, then the field node’s effect is applied to the particle as if it had a physics body. The physics body is assumed to have a mass of `1.0` and a charge of `1.0`

The default value is `0x00000000` (all bits cleared).

