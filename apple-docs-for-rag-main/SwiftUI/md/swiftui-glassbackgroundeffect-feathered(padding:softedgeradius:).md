

- SwiftUI
- GlassBackgroundEffect
-  feathered(padding:softEdgeRadius:) 

Type Method

# feathered(padding:softEdgeRadius:)

A feathered background effect with custom padding and soft edge radius.

visionOS 2.4+

``` source
static func feathered(
    padding length: CGFloat,
    softEdgeRadius: CGFloat? = nil
) -> FeatheredGlassBackgroundEffect
```

Available when `Self` is `FeatheredGlassBackgroundEffect`.

## Parameters 

`softEdgeRadius`  

When a blur is clipped, the radial size of the blur’s edge. If you set the value to `nil`, SwiftUI uses a default amount. The default value of this parameter is `nil`.

## Return Value

A feathered background effect.

