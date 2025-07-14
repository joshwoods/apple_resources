

- Core Image
- CIBlendKernel
-  luminosity 

Type Property

# luminosity

A blend kernel that uses the hue and saturation of the background image with the luminance of the foreground image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class var luminosity: CIBlendKernel { get }
```

## Discussion

Figure 1 The result of using the luminosity blend kernel (background image is top left, foreground image is bottom left)

## See Also

### Builtin Blend Kernels

class var clear: CIBlendKernel

A blend kernel that returns a clear color.

class var color: CIBlendKernel

A blend kernel that uses the luminance values of the background with the hue and saturation values of the foreground image.

class var colorBurn: CIBlendKernel

A blend kernel that darkens the background image samples to reflect the foreground image samples.

class var colorDodge: CIBlendKernel

A blend kernel that brightens the background image samples to reflect the foreground image samples.

class var componentAdd: CIBlendKernel

A blend kernel that adds color components to achieve a brightening effect.

class var componentMax: CIBlendKernel

A blend kernel that creates an image using the maximum values of two input images.

class var componentMin: CIBlendKernel

A blend kernel that creates an image using the minimum values of two input images.

class var componentMultiply: CIBlendKernel

A blend kernel that multiplies the color components of its input images.

class var darken: CIBlendKernel

A blend kernel that creates an image using the darker values of two input images.

class var darkerColor: CIBlendKernel

A blend kernel that creates an image using the darker color of two input images.

class var destination: CIBlendKernel

A blend kernel that returns the background input image.

class var destinationAtop: CIBlendKernel

A blend kernel that places the background over the foreground and crops based on the visibility of the foreground.

class var destinationIn: CIBlendKernel

A blend kernel that places the background over the foreground and crops based on the visibility of both.

class var destinationOut: CIBlendKernel

A blend kernel that uses the background image to define what to take out of the foreground image.

class var destinationOver: CIBlendKernel

A blend kernel that places the background image over the input foreground image.

class var difference: CIBlendKernel

A blend kernel that creates an image using the difference between the background and foreground images.

class var divide: CIBlendKernel

A blend kernel that divides the background image sample color with the foreground image sample color.

class var exclusion: CIBlendKernel

A blend kernel that produces an effect similar to difference blending but with lower contrast.

class var exclusiveOr: CIBlendKernel

A blend kernel that returns either the foreground or background image if the other contains a clear color.

class var hardLight: CIBlendKernel

A blend kernel that either multiplies or screens colors, depending on the source image sample color.

class var hardMix: CIBlendKernel

A blend kernel that adds two images together, setting each color channel value to either 0 or 1.

class var hue: CIBlendKernel

A blend kernel that uses the luminance and saturation values of the background image with the hue of the foreground image.

class var lighten: CIBlendKernel

A blend kernel that creates an image using the lighter values of two input images.

class var lighterColor: CIBlendKernel

A blend kernel that creates an image using the lighter color of two input images.

class var linearBurn: CIBlendKernel

A blend kernel that darkens the background image samples to reflect the foreground image samples while also increasing contrast.

class var linearDodge: CIBlendKernel

A blend kernel that lightens the background image samples to reflect the foreground image samples while also increasing contrast.

class var linearLight: CIBlendKernel

A blend kernel that burns or dodges colors by changing brightness, depending on the blend color.

class var multiply: CIBlendKernel

A blend kernel that multiplies the background image sample color with the foreground image sample color.

class var overlay: CIBlendKernel

A blend kernel that either multiplies or screens the foreground image samples with the background image samples, depending on the background color.

class var pinLight: CIBlendKernel

A blend kernel that conditionally replaces background image samples with source image samples depending on the brightness of the source image samples.

class var saturation: CIBlendKernel

A blend kernel that uses the luminance and hue values of the background image with the saturation of the foreground image.

class var screen: CIBlendKernel

A blend kernel that multiplies the inverse of the foreground image samples with the inverse of the background image samples.

class var softLight: CIBlendKernel

A blend kernel that either darkens or lightens colors, depending on the foreground image sample color.

class var source: CIBlendKernel

A blend kernel that returns the foreground input image.

class var sourceAtop: CIBlendKernel

A blend kernel that places the foreground over the background and crops based on the visibility of the background.

class var sourceIn: CIBlendKernel

A blend kernel that places the foreground over the background and crops based on the visibility of both.

class var sourceOut: CIBlendKernel

A blend kernel that uses the foreground image to define what to take out of the background image.

class var sourceOver: CIBlendKernel

A blend kernel that places the foreground image over the input background image.

class var subtract: CIBlendKernel

A blend kernel that subtracts the background image sample color from the foreground image sample color.

class var vividLight: CIBlendKernel

A blend kernel that burns or dodges colors by changing contrast, depending on the blend color.

