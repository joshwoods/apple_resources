

- SpriteKit
- SKFieldNode
-  falloff 

Instance Property

# falloff

The exponent that defines the rate of decay for the strength of the field as the distance increases between the node and the physics body being affected.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var falloff: Float { get set }
```

**watchOS**

``` source
var falloff: Float { get set }
```

## Mentioned in 

Adding Physics Fields to a Scene

## Discussion

When the force of a field node is calculated, the force is multiplied by `pow(distance - minRadius, -falloff)`. The default falloff value is `0`, which indicates that no attenuation takes place. Some types of field nodes ignore the falloff parameter entirely, while others change the default value to something that is more logical for that type of field node.

## See Also

### Configuring the Strength of the Field

var strength: Float

The strength of the field.

