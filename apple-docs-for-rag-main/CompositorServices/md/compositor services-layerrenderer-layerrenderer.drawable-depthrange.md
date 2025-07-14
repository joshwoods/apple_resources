

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
-  depthRange 

Instance Property

# depthRange

The distances to the far and near clipping planes from the person viewing the content, in meters.

visionOS 1.0+

``` source
var depthRange: simd_float2 { get nonmutating set }
```

## Discussion

Apply the depth range for drawing to the drawable that it applies to. The compositor uses these values to compute the perspective projection matrix, which clips content that’s not between the near and far planes.

Compositor Services stores the values in reverse-z order in a 2D floating-point vector:

- The `x` property stores the distance of the far plane.

- The `y` property stores the distance of the near plane.

