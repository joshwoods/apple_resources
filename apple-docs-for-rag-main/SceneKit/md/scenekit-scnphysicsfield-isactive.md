

- SceneKit
- SCNPhysicsField
-  isActive 

Instance Property

# isActive

A Boolean value that determines whether the field’s effect is enabled.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isActive: Bool { get set }
```

## Discussion

If this value is false, the field does not apply forces to physics bodies in its area of effect. The default value is true.

Use this property, for example, to switch fields on and off as a gameplay mechanic.

## See Also

### Specifying a Field’s Behavior

var strength: CGFloat

A multiplier for the force that the field applies to objects in its area of effect.

var falloffExponent: CGFloat

An exponent that determines how the field’s strength diminishes with distance.

var minimumDistance: CGFloat

The minimum value for distance-based effects.

var isExclusive: Bool

A Boolean value that determines whether the field overrides other fields whose areas of effect it overlaps.

