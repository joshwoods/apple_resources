

- Core Graphics
- CGBlendMode
-  CGBlendMode.darken 

Case

# CGBlendMode.darken

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case darken
```

## Discussion

Creates the composite image samples by choosing the darker samples (either from the source image or the background). The result is that the background image samples are replaced by any source image samples that are darker. Otherwise, the background image samples are left unchanged.

## See Also

### Constants

case normal

Paints the source image samples over the background image samples.

case multiply

Multiplies the source image samples with the background image samples. This results in colors that are at least as dark as either of the two contributing sample colors.

case screen

Multiplies the inverse of the source image samples with the inverse of the background image samples, resulting in colors that are at least as light as either of the two contributing sample colors.

case overlay

case lighten

case colorDodge

Brightens the background image samples to reflect the source image samples. Source image sample values that specify black do not produce a change.

case colorBurn

Darkens the background image samples to reflect the source image samples. Source image sample values that specify white do not produce a change.

case softLight

case hardLight

case difference

case exclusion

Produces an effect similar to that produced by CGBlendMode.difference, but with lower contrast. Source image sample values that are black don’t produce a change; white inverts the background color values.

case hue

Uses the luminance and saturation values of the background with the hue of the source image.

case saturation

Uses the luminance and hue values of the background with the saturation of the source image. Areas of the background that have no saturation (that is, pure gray areas) don’t produce a change.

case color

Uses the luminance values of the background with the hue and saturation values of the source image. This mode preserves the gray levels in the image. You can use this mode to color monochrome images or to tint color images.

case luminosity

Uses the hue and saturation of the background with the luminance of the source image. This mode creates an effect that is inverse to the effect created by CGBlendMode.color.

