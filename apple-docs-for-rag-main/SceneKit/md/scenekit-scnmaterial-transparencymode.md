

- SceneKit
- SCNMaterial
-  transparencyMode 

Instance Property

# transparencyMode

The mode SceneKit uses to calculate transparency for the material.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var transparencyMode: SCNTransparencyMode { get set }
```

## Discussion

The default transparency mode is SCNTransparencyMode.aOne. See SCNTransparencyMode for available values and their effects.

## See Also

### Managing Opacity and Blending

var transparency: CGFloat

The uniform transparency of the material. Animatable.

enum SCNTransparencyMode

The modes SceneKit uses to calculate the opacity of pixels rendered with a material, used by the transparencyMode property.

var blendMode: SCNBlendMode

The mode that determines how pixel colors rendered using this material blend with other pixel colors in the rendering target.

enum SCNBlendMode

Modes that describe how SceneKit blends source colors rendered using a material with destination colors already in a rendering target, used by the blendMode property.

