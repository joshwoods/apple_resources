

- Core Image
- Transition Filters
-  swipeTransition() 

Type Method

# swipeTransition()

Gradually transitions from one image to another with a swiping motion.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func swipeTransition() -> any CIFilter & CISwipeTransition
```

## Return Value

The transition image.

## Discussion

This method applies the swipe transition filter to an image. The effect transitions from the input image to the target image by simulating a swiping motion.

The swipe transition filter uses the following properties:

`inputImage`  
The starting image with the type CIImage.

`targetImage`  
The ending image with the type `CIImage`.

`extent`  
A CGRect representing the size of the rounded rectangle.

`time`  
A `float` representing the parametric time of the transition from start (at time 0) to end (at time 1) as an NSNumber.

angle  
A `float` representing the angle of the motion of the swipe as an `NSNumber`.

width  
A `float` representing the width of the swipe effect as an `NSNumber`.

opacity  
A `float` representing the transparency of the swipe as an `NSNumber`.

The following code creates a filter that transitions from the input image to the target image with a gradual fade from left to right.

func swipe(inputImage: CIImage, targetImage: CIImage) -> CIImage {
    let swipeTransiton = CIFilter.swipeTransition()
    swipeTransiton.inputImage = inputImage
    swipeTransiton.targetImage = targetImage
    swipeTransiton.extent = CGRect(x: 0, y: 0, width: 300, height: 300)
    swipeTransiton.time = 0.5
    swipeTransiton.angle = -0.7
    swipeTransiton.width = 203
    swipeTransiton.opacity = 0
    return swipeTransiton.outputImage!
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

class func rippleTransition() -> any CIFilter &amp; CIRippleTransition

Simulates a ripple in a pond to transiton from one image to another.

