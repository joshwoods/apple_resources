

- Core Image
- Halftone Effect Filters
-  hatchedScreen() 

Type Method

# hatchedScreen()

Creates a monochrome image with a series of lines to add detail.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func hatchedScreen() -> any CIFilter & CIHatchedScreen
```

## Return Value

The modified image.

## Discussion

This method applies a hatched screen filter to an image. The effect generates a monochrome image containing a series of lines in hatched pattern to create detail. The halftone effect is a set of lines, dots, or circles that contain detail. When viewing the image from a distance, the markings blend together, creating the illusion of continuous lines and shapes. The effect is often used in print media for more efficient printing.

The hatched screen filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

`angle`  
A `float` representing the angle of the pattern as an NSNumber.

`width`  
A `float` representing the distance between lines in the pattern as an `NSNumber`.

`sharpness`  
A `float` representing the sharpness of the pattern as an `NSNumber`.

The following code creates a filter that produces a monochrome image containing lines of detail on a black background:

func hatched(inputImage: CIImage) -> CIImage {
    let hatchedScreen = CIFilter.hatchedScreen()
    hatchedScreen.inputImage = inputImage
    hatchedScreen.center = CGPoint(x: 2016, y: 1512)
    hatchedScreen.angle = 10
    hatchedScreen.width = 35
    hatchedScreen.sharpness = 0.7
    return hatchedScreen.outputImage!
}

## See Also

### Filters

class func circularScreen() -> any CIFilter &amp; CICircularScreen

Adds a circular overlay to an image.

class func cmykHalftone() -> any CIFilter &amp; CICMYKHalftone

Adds a series of colorful dots to an image.

class func dotScreen() -> any CIFilter &amp; CIDotScreen

Creates a monochrome image with a series of dots to add detail.

class func lineScreen() -> any CIFilter &amp; CILineScreen

Creates a monochrome image with a series of small lines to add detail.

