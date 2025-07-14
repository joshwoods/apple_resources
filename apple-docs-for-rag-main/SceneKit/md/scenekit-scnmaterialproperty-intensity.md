

- SceneKit
- SCNMaterialProperty
-  intensity 

Instance Property

# intensity

A number between `0.0` and `1.0` that modulates the effect of the material property. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var intensity: CGFloat { get set }
```

## Discussion

The default intensity is `1.0`. Reducing the intensity fades out the contents of the material property, causing different effects depending on which visual property of an SCNMaterial object it represents:

- For the normal property, intensity varies the apparent roughness of the normal-mapped surface. Reducing intensity makes the surface appear more smooth.

- For the multiply property, reducing intensity blends the material property’s colors with white, effectively reducing the strength of the color multiplication effect.

- For all other properties, reducing intensity dims the material property’s contents.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Working with Material Property Contents

var contents: Any?

The visual contents of the material property—a color, image, or source of animated content. Animatable.

