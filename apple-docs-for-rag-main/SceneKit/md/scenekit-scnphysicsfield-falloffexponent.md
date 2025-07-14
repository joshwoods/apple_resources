

- SceneKit
- SCNPhysicsField
-  falloffExponent 

Instance Property

# falloffExponent

An exponent that determines how the field’s strength diminishes with distance.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var falloffExponent: CGFloat { get set }
```

## Discussion

When SceneKit calculates the force to be applied by a field, it attenuates the field’s effect by multiplying with the expression `pow(distance - minRadius, -falloff)`. If the falloff exponent is greater than zero, the field’s effect is stronger on nearby bodies than on bodies farther away from its location.

The default falloff exponent varies by field type. For details, see the methods listed in Creating Physics Fields.

## See Also

### Specifying a Field’s Behavior

var strength: CGFloat

A multiplier for the force that the field applies to objects in its area of effect.

var minimumDistance: CGFloat

The minimum value for distance-based effects.

var isActive: Bool

A Boolean value that determines whether the field’s effect is enabled.

var isExclusive: Bool

A Boolean value that determines whether the field overrides other fields whose areas of effect it overlaps.

