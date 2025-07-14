

- SpriteKit
- SKFieldNode
-  strength 

Instance Property

# strength

The strength of the field.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
var strength: Float { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var strength: Float { get set }
```

## Mentioned in 

Adding Physics Fields to a Scene

## Discussion

The default value is `1.0`. There’s no specific unit of measurement for this property because the actual effect is dependent on the kind of field node being created. In practice, the best approach is to experiment with different field strengths and use them to determine the proper value empirically.

## See Also

### Configuring the Strength of the Field

var falloff: Float

The exponent that defines the rate of decay for the strength of the field as the distance increases between the node and the physics body being affected.

