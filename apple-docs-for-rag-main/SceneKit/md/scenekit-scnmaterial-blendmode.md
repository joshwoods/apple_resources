

- SceneKit
- SCNMaterial
-  blendMode 

Instance Property

# blendMode

The mode that determines how pixel colors rendered using this material blend with other pixel colors in the rendering target.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var blendMode: SCNBlendMode { get set }
```

## Discussion

With the default blend mode of SCNBlendMode.alpha, materials blend according to their alpha (opacity) values—a pixel rendered with a higher alpha value appears more opaque than one with a lower alpha value. Change this property to create special effects. For example, the SCNBlendMode.add mode can make objects appear to glow.

## See Also

### Managing Opacity and Blending

var transparency: CGFloat

The uniform transparency of the material. Animatable.

var transparencyMode: SCNTransparencyMode

The mode SceneKit uses to calculate transparency for the material.

enum SCNTransparencyMode

The modes SceneKit uses to calculate the opacity of pixels rendered with a material, used by the transparencyMode property.

enum SCNBlendMode

Modes that describe how SceneKit blends source colors rendered using a material with destination colors already in a rendering target, used by the blendMode property.

