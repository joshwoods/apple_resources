

- SceneKit
- SCNMaterial
-  isLitPerPixel 

Instance Property

# isLitPerPixel

A Boolean value that determines whether SceneKit performs lighting calculations per vertex or per pixel. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isLitPerPixel: Bool { get set }
```

## Discussion

When this property’s value is true (the default), SceneKit performs lighting calculations independently for each rendered pixel. This approach provides better rendering quality, but can adversely impact rendering performance.

If you change this property’s value to false, SceneKit performs lighting calculations for each vertex in a geometry, and allows the GPU to interpolate lighting results across the pixels in between vertices. Depending on the shape and vertex count of a geometry’s surface and the material properties being rendered, this approach may improve rendering performance without much noticeable impact on visual quality.

You can animate changes to this property’s value. See Animating SceneKit Content. Animating this property fades between the results of rendering with each state.

## See Also

### Customizing Rendered Appearance

var isDoubleSided: Bool

A Boolean value that determines whether SceneKit renders both front and back faces of a surface.

var cullMode: SCNCullMode

The mode determining which faces of a surface SceneKit renders. Animatable.

enum SCNCullMode

The modes SceneKit uses to determine which polygons to render in a surface, used by the cullMode property.

var fillMode: SCNFillMode

enum SCNFillMode

