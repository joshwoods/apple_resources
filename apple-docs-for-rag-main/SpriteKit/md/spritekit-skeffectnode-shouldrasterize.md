

- SpriteKit
- SKEffectNode
-  shouldRasterize 

Instance Property

# shouldRasterize

A Boolean value that indicates whether the results of rendering the child nodes should be cached.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var shouldRasterize: Bool { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var shouldRasterize: Bool { get set }
```

## Mentioned in 

Creating a New Node By Rendering To a Texture

## Discussion

If the value of this property is true, the effect node caches the filtered image for use in future frames. If the value is false, then SpriteKit discards the rendered image and redraws it from scratch the next time the node is rendered. The default value is false. Caching the rendered image uses more memory and may take more time to render. However, if the effect node’s descendants rarely change, caching can improve performance.

When caching is enabled, changes to the effect node’s children trigger updates to the cached image in the next frame of animation. However, changing the filter’s properties does not.

## See Also

### Flattening an Effect Node’s Child Tree for Performance Improvement

Improving the Performance of Static Content

Flatten a portion of your node hierarchy to a single texture to improve performance.

