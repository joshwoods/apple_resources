

- SceneKit
- SCNMaterial
-  isDoubleSided 

Instance Property

# isDoubleSided

A Boolean value that determines whether SceneKit renders both front and back faces of a surface.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isDoubleSided: Bool { get set }
```

## Discussion

Polygons in a SceneKit mesh are, by default, single-sided. Each one contain a *normal vector*, which identifies the side of the polygon that’s the visible side. SceneKit uses that normal vector to determine which polygons are *front faces* that point toward the camera, and which are *back faces* that point away from it. When `doubleSided` is false (the default value), SceneKit only renders front faces to improve performance.

If you change this property’s value to true, SceneKit renders both the front and back surfaces of every polygon.

You can animate changes to this property’s value. See Animating SceneKit Content. Animating this property fades between the results of rendering with each state.

## See Also

### Customizing Rendered Appearance

var isLitPerPixel: Bool

A Boolean value that determines whether SceneKit performs lighting calculations per vertex or per pixel. Animatable.

var cullMode: SCNCullMode

The mode determining which faces of a surface SceneKit renders. Animatable.

enum SCNCullMode

The modes SceneKit uses to determine which polygons to render in a surface, used by the cullMode property.

var fillMode: SCNFillMode

enum SCNFillMode

