

- Core Animation
- CAReplicatorLayer
-  instanceGreenOffset 

Instance Property

# instanceGreenOffset

Defines the offset added to the green component of the color for each replicated instance. Animatable.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var instanceGreenOffset: Float { get set }
```

## Discussion

The `instanceGreenOffset` is added to the green color component of instance `k-1` to produce the modulation color of instance k.

Default is `0.0`.

## See Also

### Accessing Instance Color Values

var instanceColor: CGColor?

Defines the color used to multiply the source object. Animatable.

var instanceRedOffset: Float

Defines the offset added to the red component of the color for each replicated instance. Animatable.

var instanceBlueOffset: Float

Defines the offset added to the blue component of the color for each replicated instance. Animatable.

var instanceAlphaOffset: Float

Defines the offset added to the alpha component of the color for each replicated instance. Animatable.

