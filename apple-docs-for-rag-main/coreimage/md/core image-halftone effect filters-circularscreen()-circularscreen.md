

- Core Image
- Halftone Effect Filters
-  circularScreen() 

Type Method

# circularScreen()

Adds a circular overlay to an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func circularScreen() -> any CIFilter & CICircularScreen
```

## Return Value

The modified image.

## Discussion

This method applies a circular screen filter to an image. The effect generates a monochrome image containing a series of circular rings. The halftone effect is a set of lines, dots, or circles that contain detail. When viewing the image from a distance, the markings blend together, creating the illusion of continuous lines and shapes. Print media commonly uses this effect.

The circular screen filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

`width`  
A `float` representing the distance between each circle in the pattern as an NSNumber.

`sharpness`  
A `float` representing the sharpness of the circles in the pattern as an `NSNumber`.

The following code creates a filter that results in a monochrome image with a large circular pattern overlaying the image:

func circular(inputImage: CIImage) -> CIImage {
    let circularHalftone = CIFilter.circularScreen()
    circularHalftone.inputImage = inputImage
    circularHalftone.center = CGPoint(x: 2016, y: 1512)
    circularHalftone.width = 35
    circularHalftone.sharpness = 0.70
    return circularHalftone.outputImage!
}

## See Also

### Filters

class func cmykHalftone() -> any CIFilter &amp; CICMYKHalftone

Adds a series of colorful dots to an image.

class func dotScreen() -> any CIFilter &amp; CIDotScreen

Creates a monochrome image with a series of dots to add detail.

class func hatchedScreen() -> any CIFilter &amp; CIHatchedScreen

Creates a monochrome image with a series of lines to add detail.

class func lineScreen() -> any CIFilter &amp; CILineScreen

Creates a monochrome image with a series of small lines to add detail.

