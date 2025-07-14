

- SceneKit
- SCNPhysicsField
-  isExclusive 

Instance Property

# isExclusive

A Boolean value that determines whether the field overrides other fields whose areas of effect it overlaps.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isExclusive: Bool { get set }
```

## Discussion

If this value is true and a physics body is within this field’s region, SceneKit ignores the effects of all other fields that might otherwise affect the body. The default value is false.

If you set this property to true on multiple fields in a scene, their regions should not overlap. If they do, the results are undefined.

## See Also

### Specifying a Field’s Behavior

var strength: CGFloat

A multiplier for the force that the field applies to objects in its area of effect.

var falloffExponent: CGFloat

An exponent that determines how the field’s strength diminishes with distance.

var minimumDistance: CGFloat

The minimum value for distance-based effects.

var isActive: Bool

A Boolean value that determines whether the field’s effect is enabled.

