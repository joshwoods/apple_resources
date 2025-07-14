

- Core Image
- Color Effect Filters
-  colorCube() 

Type Method

# colorCube()

Adjusts an image’s pixels using a three-dimensional color table.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func colorCube() -> any CIFilter & CIColorCube
```

## Return Value

The modified image.

## Discussion

This method applies the color cube filter to an image. The effect maps color values in the input image to new color values using a three-dimensional color look-up table, also called a color cube. For each `RGBA` pixel in the input image, the filter uses the pixel’s `red`, `green`, and `blue` component values to identify a location in the table. The `RGBA` value at that location becomes the `RGBA` value of the output pixel.

The color cube filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`cubeData`  
Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.

`extrapolate`  
If `true`, then the filter extrapolates the color cube for any RGB component values outside the range 0.0 to 1.0.

`cubeDimension`  
The dimension of the color cube.

The following code creates a filter that adds a blue hue to the input image:

func colorCube(inputImage: CIImage, cubeData: Data) -> CIImage {
    let colorCubeEffect = CIFilter.colorCube()
    colorCubeEffect.inputImage = inputImage
    colorCubeEffect.cubeData = cubeData
    colorCubeEffect.cubeDimension = 4
    return colorCubeEffect.outputImage!
}
// Create a color cube with size 4.
var colorCubeData: [Float32] = []
let size = 4
let step = 1.0 / Float(size - 1)
for b in 0..&lt;size {
    for g in 0..&lt;size {
        for r in 0..&lt;size {
            // Calculate the normalized color component values.
            let red = Float32(r) * step
            let green = Float32(g) * step
            // Shift the blue component to add a blue tint.
            let blue = min(1.0, Float32(b) * step + 0.5)
            let alpha: Float = 1.0
            colorCubeData.append(contentsOf: [red, green, blue, alpha])
        }
    }
}
let cubeData = Data(bytes: colorCubeData, count: colorCubeData.count * 4)
let result = colorCube(inputImage: ciImage, cubeData: cubeData)
imageView.image = UIImage(ciImage: result)

## See Also

### Color Effect Filters

class func colorCrossPolynomial() -> any CIFilter &amp; CIColorCrossPolynomial

Adjusts an image’s color by applying polynomial cross-products.

class func colorCubeWithColorSpace() -> any CIFilter &amp; CIColorCubeWithColorSpace

Adjusts an image’s pixels using a three-dimensional color table in specified color space.

class func colorCubesMixedWithMask() -> any CIFilter &amp; CIColorCubesMixedWithMask

Alters an image’s pixels using a three-dimensional color tables and a mask image.

class func colorCurves() -> any CIFilter &amp; CIColorCurves

Adjusts an image’s color curves.

class func colorInvert() -> any CIFilter &amp; CIColorInvert

Inverts an image’s colors.

class func colorMap() -> any CIFilter &amp; CIColorMap

Performs a transformation of the input image colors to colors from a gradient image.

class func colorMonochrome() -> any CIFilter &amp; CIColorMonochrome

Adjusts an image’s colors to shades of a single color.

class func colorPosterize() -> any CIFilter &amp; CIColorPosterize

Flattens an image’s colors.

class func convertLabToRGB() -> any CIFilter &amp; CIConvertLab

Converts an image from CIELAB to RGB color space.

class func convertRGBtoLab() -> any CIFilter &amp; CIConvertLab

Converts an image from RGB to CIELAB color space.

class func dither() -> any CIFilter &amp; CIDither

Applies randomized noise to produce a processed look.

class func documentEnhancer() -> any CIFilter &amp; CIDocumentEnhancer

Adjusts an image’s shadows and contrast.

class func falseColor() -> any CIFilter &amp; CIFalseColor

Replaces an image’s colors with specified colors.

class func labDeltaE() -> any CIFilter &amp; CILabDeltaE

Compares an image’s color values.

class func maskToAlpha() -> any CIFilter &amp; CIMaskToAlpha

Converts an image to a white image with an alpha component.

class func maximumComponent() -> any CIFilter &amp; CIMaximumComponent

Creates a maximum RGB grayscale image.

class func minimumComponent() -> any CIFilter &amp; CIMinimumComponent

Creates a minimum RGB grayscale image.

class func paletteCentroid() -> any CIFilter &amp; CIPaletteCentroid

Calculates the location of an image’s colors.

class func palettize() -> any CIFilter &amp; CIPalettize

Replaces colors with colors from a palette image.

class func photoEffectChrome() -> any CIFilter &amp; CIPhotoEffect

Exaggerates an image’s colors.

class func photoEffectFade() -> any CIFilter &amp; CIPhotoEffect

Diminishes an image’s colors.

class func photoEffectInstant() -> any CIFilter &amp; CIPhotoEffect

Desaturates an image’s colors.

class func photoEffectMono() -> any CIFilter &amp; CIPhotoEffect

Adjust an image’s colors to black and white.

class func photoEffectNoir() -> any CIFilter &amp; CIPhotoEffect

Adjusts an image’s colors to black and white and intensifies the contrast.

class func photoEffectProcess() -> any CIFilter &amp; CIPhotoEffect

Lowers the contrast of the input image.

class func photoEffectTonal() -> any CIFilter &amp; CIPhotoEffect

Adjusts an image’s colors to black and white.

class func photoEffectTransfer() -> any CIFilter &amp; CIPhotoEffect

Brightens an image’s colors.

class func sepiaTone() -> any CIFilter &amp; CISepiaTone

Adjusts an image’s colors to shades of brown.

class func thermal() -> any CIFilter &amp; CIThermal

Alters the image to make it look like it was taken by a thermal camera.

class func vignette() -> any CIFilter &amp; CIVignette

Gradually darkens an image’s edges.

class func vignetteEffect() -> any CIFilter &amp; CIVignetteEffect

Gradually darkens a specified area of an image.

class func xRay() -> any CIFilter &amp; CIXRay

Alters an image to make it look like an X-ray image.

