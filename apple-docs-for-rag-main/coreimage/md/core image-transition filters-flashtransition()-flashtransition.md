

- Core Image
- Transition Filters
-  flashTransition() 

Type Method

# flashTransition()

Creates a flash of light to transition between two images.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func flashTransition() -> any CIFilter & CIFlashTransition
```

## Return Value

The transition image.

## Discussion

This method applies the flash transition filter to an image. The effect transitions from the input image to the target image by creating a flash that fills the image and fades to the target image.

The flash transition filter uses the following properties:

`inputImage`  
The starting image with the type CIImage.

`targetImage`  
The ending image with the type `CIImage`.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

`extent`  
A CGRect representing the size of the rounded rectangle.

`color`  
A CIColor representing the color of the flash effect.

`time`  
A `float` representing the parametric time of the transition from start (at time 0) to end (at time 1) as an NSNumber.

`maxStiriationRadius`  
A `float` representing the radius of the light rays emanating from the flash as a `NSNumber`.

`striationStrength`  
A `float` representing the strength of the light rays emanating from the flash as a `NSNumber`.

`striationContrast`  
A `float` representing the contrast that’s added to each output pixel as a `NSNumber`.

`fadeThreshold`  
A `float` representing the amount of fade between the flash and the target image as a `NSNumber`.

The following code creates a filter that transitions from the input image with a large flash of light and fades to the target image.

func flash (inputImage: CIImage, targetImage: CIImage) -> CIImage {
    let flashTransition = CIFilter.flashTransition()
    flashTransition.inputImage = inputImage
    flashTransition.targetImage = targetImage
    flashTransition.center = CGPoint(x: 253, y: 372)
    flashTransition.extent = CGRect(x: 0, y: 0, width: 300, height: 300)
    flashTransition.color = .white
    flashTransition.time = 0.5
    flashTransition.maxStriationRadius = 2.58
    flashTransition.striationStrength = 0.5
    flashTransition.striationContrast = 1.375
    flashTransition.fadeThreshold = 0.06
    return flashTransition.outputImage!
}

## See Also

### Filters

class func accordionFoldTransition() -> any CIFilter &amp; CIAccordionFoldTransition

Transitions by folding and crossfading an image to reveal the target image.

class func barsSwipeTransition() -> any CIFilter &amp; CIBarsSwipeTransition

Transitions between two images by removing rectangular portions of an image.

class func copyMachineTransition() -> any CIFilter &amp; CICopyMachineTransition

Simulates the effect of a copy machine scanner light to transiton between two images.

class func disintegrateWithMaskTransition() -> any CIFilter &amp; CIDisintegrateWithMaskTransition

Transitions between two images using a mask image.

class func dissolveTransition() -> any CIFilter &amp; CIDissolveTransition

Transitions between two images with a fade effect.

class func modTransition() -> any CIFilter &amp; CIModTransition

Transitions between two images by applying irregularly shaped holes.

class func pageCurlTransition() -> any CIFilter &amp; CIPageCurlTransition

Simulates the curl of a page, revealing the target image.

class func pageCurlWithShadowTransition() -> any CIFilter &amp; CIPageCurlWithShadowTransition

Simulates the curl of a page, revealing the target image with added shadow.

class func rippleTransition() -> any CIFilter &amp; CIRippleTransition

Simulates a ripple in a pond to transiton from one image to another.

class func swipeTransition() -> any CIFilter &amp; CISwipeTransition

Gradually transitions from one image to another with a swiping motion.

