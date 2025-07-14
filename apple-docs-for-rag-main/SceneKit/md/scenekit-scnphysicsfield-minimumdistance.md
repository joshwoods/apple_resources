

- SceneKit
- SCNPhysicsField
-  minimumDistance 

Instance Property

# minimumDistance

The minimum value for distance-based effects.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var minimumDistance: CGFloat { get set }
```

## Discussion

This property determines the beginning of the field’s falloff area. At distances less than the minimum, the field’s effect is at full strength. At greater distances, the field’s effect diminishes based on the value of the falloffExponent property. The default minimum distance is a very small (but nonzero) value.

## See Also

### Specifying a Field’s Behavior

var strength: CGFloat

A multiplier for the force that the field applies to objects in its area of effect.

var falloffExponent: CGFloat

An exponent that determines how the field’s strength diminishes with distance.

var isActive: Bool

A Boolean value that determines whether the field’s effect is enabled.

var isExclusive: Bool

A Boolean value that determines whether the field overrides other fields whose areas of effect it overlaps.

