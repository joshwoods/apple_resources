

- Core Image
- Color Effect Filters
-  colorCubesMixedWithMask() 

Type Method

# colorCubesMixedWithMask()

Alters an image’s pixels using a three-dimensional color tables and a mask image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func colorCubesMixedWithMask() -> any CIFilter & CIColorCubesMixedWithMask
```

## Return Value

The modified image.

## Discussion

This method applies the color cubes mixed with mask filter to an image. The effect uses two color cube tables to modify the input image. The filter uses the mask image to interpolate between the two color cubes.

The color cubes mixed with mask filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`maskImage`  
A mask image with the type `CIImage`.

`cube0Data`  
Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.

`cube1Data`  
Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.

`colorSpace`  
A CGColorSpace representing the color space for the color cubes.

`cubeDimension`  
The dimension of the color cubes

The following code creates a filter that adds colors from the mask image and brightness to the input image:

func colorCube(inputImage: CIImage, maskImage: CIImage, cube0Data: Data, cube1Data: Data) -> CIImage {
    let colorCubeEffect = CIFilter.colorCubesMixedWithMask()
    colorCubeEffect.inputImage = inputImage
    colorCubeEffect.colorSpace = CGColorSpaceCreateDeviceRGB()
    colorCubeEffect.cube0Data = cube1Data
    colorCubeEffect.cube1Data = cube0Data
    colorCubeEffect.maskImage = maskImage
    colorCubeEffect.cubeDimension = 4
    return colorCubeEffect.outputImage!
}
var colorCube0Data: [Float32] = []
var colorCube1Data: [Float32] = []
let size = 4
let step = 1.0 / Float(size - 1)
for b in 0..&lt;size {
    for g in 0..&lt;size {
        for r in 0..&lt;size {
            // Calculate the normalized color component values.
            let redNormalised = Float32(r) * step
            let greenNormalised = Float32(g) * step
            let blueNormalised = Float32(b) * step
            let alpha: Float = 1.0
            colorCube0Data.append(contentsOf: [redNormalised*1.2, greenNormalised*0.8, blueNormalised*1.2, alpha])
            colorCube1Data.append(contentsOf: [redNormalised*1.2, greenNormalised*1.15, blueNormalised*0.9, alpha])
        }
    }
}
let cube0Data = Data(bytes:colorCube0Data, count: colorCube0Data.count*4)
let cube1Data = Data(bytes:colorCube1Data, count: colorCube1Data.count*4)
let maskImage = CIFilter.linearGradient()
maskImage.color0 = CIColor(red: 1.0, green: 1.0, blue: 1.0, alpha: 1.0)
maskImage.color1 = CIColor(red: 0.0, green: 0.0, blue: 0.0, alpha: 0.0)
maskImage.point0 = CGPoint(x:0, y:0)
maskImage.point1 = CGPoint(x: ciImage.extent.width, y: 0)
let result = colorCube(inputImage: ciImage, maskImage: maskImage.outputImage!, cube0Data: cube0Data, cube1Data: cube1Data)

## See Also

### Color Effect Filters

class func colorCrossPolynomial() -> any CIFilter &amp; CIColorCrossPolynomial

Adjusts an image’s color by applying polynomial cross-products.

class func colorCube() -> any CIFilter &amp; CIColorCube

Adjusts an image’s pixels using a three-dimensional color table.

class func colorCubeWithColorSpace() -> any CIFilter &amp; CIColorCubeWithColorSpace

Adjusts an image’s pixels using a three-dimensional color table in specified color space.

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

