

- Core Image
- Halftone Effect Filters
-  cmykHalftone() 

Type Method

# cmykHalftone()

Adds a series of colorful dots to an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func cmykHalftone() -> any CIFilter & CICMYKHalftone
```

## Return Value

The modified image.

## Discussion

This method applies a CMYK halftone filter to an image. The effect generates an image containing a series of dots. The dots contain only cyan, magenta, yellow, and black colors. Halftone effect is a set of lines, dots, or circles that contain detail. When viewing the image from a distance, the markings blend together creating the illusion of continuous lines and shapes. Print media commonly uses this effect.

The CMYK halftone filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`angle`  
A `float` representing the angle of the pattern as an NSNumber.

`width`  
A `float` representing the distance between dots in the pattern as an `NSNumber`.

`sharpness`  
A `float` representing the sharpness of the pattern as an `NSNumber`.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

`grayComponentReplacement`  
A `float` representing the grey component to be replaced as an `NSNumber`.

`underColorRemoval`  
A `float` representing the under-color removal value as an `NSNumber`.

The following code produces an image with visible dots and less color:

func cmyk(inputImage: CIImage) -> CIImage {
    let cmykHalftone = CIFilter.cmykHalftone()
    cmykHalftone.inputImage = inputImage
    cmykHalftone.angle = 1
    cmykHalftone.width = 35
    cmykHalftone.sharpness = 0.7
    cmykHalftone.center = CGPoint(x: 2016, y: 1512)
    cmykHalftone.grayComponentReplacement = 1
    cmykHalftone.underColorRemoval = 0.1
    return cmykHalftone.outputImage!
}

## See Also

### Filters

class func circularScreen() -> any CIFilter &amp; CICircularScreen

Adds a circular overlay to an image.

class func dotScreen() -> any CIFilter &amp; CIDotScreen

Creates a monochrome image with a series of dots to add detail.

class func hatchedScreen() -> any CIFilter &amp; CIHatchedScreen

Creates a monochrome image with a series of lines to add detail.

class func lineScreen() -> any CIFilter &amp; CILineScreen

Creates a monochrome image with a series of small lines to add detail.

