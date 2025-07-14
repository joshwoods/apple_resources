

- SceneKit
- SCNPhysicsField
-  strength 

Instance Property

# strength

A multiplier for the force that the field applies to objects in its area of effect.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var strength: CGFloat { get set }
```

## Discussion

Each type of physics field defines its own behavior for strength values. For details, see the methods listed in Creating Physics Fields.

## See Also

### Specifying a Field’s Behavior

var falloffExponent: CGFloat

An exponent that determines how the field’s strength diminishes with distance.

var minimumDistance: CGFloat

The minimum value for distance-based effects.

var isActive: Bool

A Boolean value that determines whether the field’s effect is enabled.

var isExclusive: Bool

A Boolean value that determines whether the field overrides other fields whose areas of effect it overlaps.

