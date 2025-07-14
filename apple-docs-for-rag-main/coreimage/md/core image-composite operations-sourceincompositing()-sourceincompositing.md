

- Core Image
- Composite Operations
-  sourceInCompositing() 

Type Method

# sourceInCompositing()

Subtracts non-overlapping areas of two images, resulting in one image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func sourceInCompositing() -> any CIFilter & CICompositeOperation
```

## Return Value

The modified image.

## Discussion

This method applies the source-in compositing filter to an image. The effect creates the result by overlaying the input image over the background image. The filter then removes the non-overlapping area of both images.

The source-in compositing filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`backgroundImage`  
An image with the type `CIImage`.

The following code creates a filter that results in an output image that shows the portion of the background image that overlaps with the input:

func sourceInCompositing(inputImage: CIImage, backgroundImage: CIImage) -> CIImage {
    let colorBlendFilter = CIFilter.sourceInCompositing()
    colorBlendFilter.inputImage = inputImage
    colorBlendFilter.backgroundImage = backgroundImage
    return colorBlendFilter.outputImage!
}

## See Also

### Filters

class func additionCompositing() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images by addition.

class func colorBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images using the luminance values from the background image and the hue and saturation values from the input image.

class func colorBurnBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images while darkening the image.

class func colorDodgeBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images using dodging.

class func darkenBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images while darkening lighter pixels.

class func differenceBlendMode() -> any CIFilter &amp; CICompositeOperation

Subtracts color values to blend colors.

class func divideBlendMode() -> any CIFilter &amp; CICompositeOperation

Divides color values to blend colors.

class func exclusionBlendMode() -> any CIFilter &amp; CICompositeOperation

Subtracts color values to blend colors with less contrast.

class func hardLightBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images by screening and multiplying.

class func hueBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images by computing the sum of image color values.

class func lightenBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images by brightening colors.

class func linearBurnBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images while increasing contrast.

class func linearDodgeBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images with dodging.

class func linearLightBlendMode() -> any CIFilter &amp; CICompositeOperation

A combination of linear burn and linear dodge blend modes.

class func luminosityBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images by calculating the color, hue, and saturation.

class func minimumCompositing() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images by computing minimum values.

class func maximumCompositing() -> any CIFilter &amp; CICompositeOperation

Applies a maximum compositing filter to an image.

class func multiplyBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images by multiplying color components.

class func multiplyCompositing() -> any CIFilter &amp; CICompositeOperation

Blurs the colors of two images by multiplying color components.

class func overlayBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors by overlaying images.

class func pinLightBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images by replacing brighter colors.

class func saturationBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends the colors and saturation values of two images.

class func screenBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images by multiplying colors.

class func softLightBlendMode() -> any CIFilter &amp; CICompositeOperation

Blurs the colors of two images by calculating luminance.

class func sourceAtopCompositing() -> any CIFilter &amp; CICompositeOperation

Overlaps two images to create one cropped image.

class func sourceOutCompositing() -> any CIFilter &amp; CICompositeOperation

Subtracts overlapping area of two images to create the output image.

class func sourceOverCompositing() -> any CIFilter &amp; CICompositeOperation

Places one image over a second image.

class func subtractBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors by subtracting color values from two images.

class func vividLightBlendMode() -> any CIFilter &amp; CICompositeOperation

A combination of color-burn and color-dodge blend modes.

