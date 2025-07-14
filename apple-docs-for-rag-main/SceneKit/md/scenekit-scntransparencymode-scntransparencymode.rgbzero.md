

- SceneKit
- SCNTransparencyMode
-  SCNTransparencyMode.rgbZero 

Case

# SCNTransparencyMode.rgbZero

SceneKit derives transparency information from the luminance of colors. The value `0.0` is opaque.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case rgbZero
```

## Discussion

When using this mode, SceneKit ignores the alpha value of colors in the material’s transparent property. SceneKit calculates the luminance of a color from its red, green, and blue channels and uses the resulting value to determine the material’s opacity.

## See Also

### Constants

case aOne

SceneKit derives transparency information from the alpha channel of colors. The value `1.0` is opaque.

