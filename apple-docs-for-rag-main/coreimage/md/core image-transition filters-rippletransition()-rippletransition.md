

- Core Image
- Transition Filters
-  rippleTransition() 

Type Method

# rippleTransition()

Simulates a ripple in a pond to transiton from one image to another.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func rippleTransition() -> any CIFilter & CIRippleTransition
```

## Return Value

The transition image.

## Discussion

This method applies the ripple transition filter to an image. The effect transitions from one image to another by creating a circular wave that expands from the center point, revealing the target image through the wave effect.

The ripple transition filter uses the following properties:

`inputImage`  
The starting image with the type CIImage.

`targetImage`  
The ending image with the type `CIImage`.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

`width`  
A `float` representing the width of the ripple effect as an NSNumber.

`extent`  
A CGRect representing the size of the ripple effect.

`scale`  
A `float` representing the scale of the effect as an `NSNumber`.

`time`  
A `float` representing the parametric time of the transition from start (at time 0) to end (at time 1) as an `NSNumber`.

The following code creates a filter that transitions from the input image to the target image with a water-like ripple effect.

func ripple (inputImage: CIImage, targetImage: CIImage) -> CIImage {
    let rippleTransition = CIFilter.rippleTransition()
    rippleTransition.inputImage = inputImage
    rippleTransition.targetImage = targetImage
    rippleTransition.center = CGPoint(x: 250, y: 150)
    rippleTransition.width = 100
    rippleTransition.extent = CGRect(x: 54, y: 80, width: 300, height: 300)
    rippleTransition.scale = 22
    rippleTransition.time = 0.3
    return rippleTransition.outputImage!
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

class func flashTransition() -> any CIFilter &amp; CIFlashTransition

Creates a flash of light to transition between two images.

class func modTransition() -> any CIFilter &amp; CIModTransition

Transitions between two images by applying irregularly shaped holes.

class func pageCurlTransition() -> any CIFilter &amp; CIPageCurlTransition

Simulates the curl of a page, revealing the target image.

class func pageCurlWithShadowTransition() -> any CIFilter &amp; CIPageCurlWithShadowTransition

Simulates the curl of a page, revealing the target image with added shadow.

class func swipeTransition() -> any CIFilter &amp; CISwipeTransition

Gradually transitions from one image to another with a swiping motion.

