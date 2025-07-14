

- SceneKit
- SCNMaterial
-  transparency 

Instance Property

# transparency

The uniform transparency of the material. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var transparency: CGFloat { get set }
```

## Discussion

SceneKit determines the total opacity of each rendered pixel in a surface by multiplying the color from the material’s transparent property by the value of this property. Then, the material’s transparencyMode property determines how pixels from the material are blended into the scene.

You can also uniformly adjust the opacity of all content attached to a node using its opacity property.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Opacity and Blending

var transparencyMode: SCNTransparencyMode

The mode SceneKit uses to calculate transparency for the material.

enum SCNTransparencyMode

The modes SceneKit uses to calculate the opacity of pixels rendered with a material, used by the transparencyMode property.

var blendMode: SCNBlendMode

The mode that determines how pixel colors rendered using this material blend with other pixel colors in the rendering target.

enum SCNBlendMode

Modes that describe how SceneKit blends source colors rendered using a material with destination colors already in a rendering target, used by the blendMode property.

