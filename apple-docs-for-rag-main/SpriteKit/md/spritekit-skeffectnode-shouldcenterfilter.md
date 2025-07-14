

- SpriteKit
- SKEffectNode
-  shouldCenterFilter 

Instance Property

# shouldCenterFilter

A Boolean value that determines whether the effect node automatically sets the filter’s image center.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var shouldCenterFilter: Bool { get set }
```

**watchOS**

``` source
var shouldCenterFilter: Bool { get set }
```

## Discussion

If the value of this property is true and the filter has an `inputCenter` parameter, the effect node automatically sets the filter’s input center to the effect node’s origin. The default value is true.

## See Also

### Applying Core Image Filters with an Effect Node

Applying Special Effects to a Node’s Children

Apply the Core Image suite of filters to child nodes of an effect node.

var filter: CIFilter?

The Core Image filter to apply.

var shouldEnableEffects: Bool

A Boolean value that determines whether the effect node applies the filter to its children as they are drawn.

