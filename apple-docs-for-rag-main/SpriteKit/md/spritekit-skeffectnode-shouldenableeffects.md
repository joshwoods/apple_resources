

- SpriteKit
- SKEffectNode
-  shouldEnableEffects 

Instance Property

# shouldEnableEffects

A Boolean value that determines whether the effect node applies the filter to its children as they are drawn.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var shouldEnableEffects: Bool { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var shouldEnableEffects: Bool { get set }
```

## Discussion

If the value of this property is true, the effect node applies the filter and blends the results. If the value is false, the effect node is ignored and its children are rendered normally. The default value is false.

## See Also

### Applying Core Image Filters with an Effect Node

Applying Special Effects to a Node’s Children

Apply the Core Image suite of filters to child nodes of an effect node.

var filter: CIFilter?

The Core Image filter to apply.

var shouldCenterFilter: Bool

A Boolean value that determines whether the effect node automatically sets the filter’s image center.

