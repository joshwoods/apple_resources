

- Core Image
- Halftone Effect Filters
-  dotScreen() 

Type Method

# dotScreen()

Creates a monochrome image with a series of dots to add detail.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func dotScreen() -> any CIFilter & CIDotScreen
```

## Return Value

The modified image.

## Discussion

This method applies a dot screen filter to an image. The effect generates a monochrome image containing a series of dots creating detail. The halftone effect is a set of lines, dots, or circles that contain detail. When viewing the image from a distance, the markings blend together, creating the illusion of continuous lines and shapes. Print media commonly uses this effect.

The dot screen filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

`width`  
A `float` representing the distance between dots in the pattern as an NSNumber.

`sharpness`  
A `float` representing the sharpness of the pattern as an `NSNumber`.

The following code creates a filter that produces an image containing monochrome dots of detail on a black background:

func dot (inputImage: CIImage) -> CIImage {
    let dotScreen = CIFilter.dotScreen()
    dotScreen.inputImage = inputImage
    dotScreen.angle = 0
    dotScreen.center = CGPoint(x: 2016, y: 1512)
    dotScreen.width = 35
    dotScreen.sharpness = 0.7
    return dotScreen.outputImage!
}

## See Also

### Filters

class func circularScreen() -> any CIFilter &amp; CICircularScreen

Adds a circular overlay to an image.

class func cmykHalftone() -> any CIFilter &amp; CICMYKHalftone

Adds a series of colorful dots to an image.

class func hatchedScreen() -> any CIFilter &amp; CIHatchedScreen

Creates a monochrome image with a series of lines to add detail.

class func lineScreen() -> any CIFilter &amp; CILineScreen

Creates a monochrome image with a series of small lines to add detail.

