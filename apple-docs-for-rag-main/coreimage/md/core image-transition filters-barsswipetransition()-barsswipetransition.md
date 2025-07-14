

- Core Image
- Transition Filters
-  barsSwipeTransition() 

Type Method

# barsSwipeTransition()

Transitions between two images by removing rectangular portions of an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func barsSwipeTransition() -> any CIFilter & CIBarsSwipeTransition
```

## Return Value

The transition image.

## Discussion

This method applies the bar swipe transition filter to an image. The effect transitions from one image to another by a series of moving bars passing over the target image.

The bar swipe transition filter uses the following properties:

`inputImage`  
The starting image with the type CIImage.

`targetImage`  
The ending image with the type `CIImage`.

`time`  
A `float` representing the parametric time of the transition from start (at time 0) to end (at time 1) as an NSNumber.

`angle`  
A `float` representing the angle of the motion as an `NSNumber`.

`width`  
A `float` representing the width of the bars in pixels as an `NSNumber`.

`barOffset`  
A `float` representing the offset of one bar in relation to others as a `NSNumber`.

The following code creates a filter that produces falling bars from the input image to transition to the target image:

func barSwipe(inputImage: CIImage, targetImage: CIImage) -> CIImage {
    let barSwipeTranstion = CIFilter.barsSwipeTransition()
    barSwipeTranstion.inputImage = inputImage
    barSwipeTranstion.targetImage = targetImage
    barSwipeTranstion.time = 0.5
    barSwipeTranstion.angle = 0.09
    barSwipeTranstion.width = 30
    barSwipeTranstion.barOffset = 10   
    return barSwipeTranstion.outputImage!
}

## See Also

### Filters

class func accordionFoldTransition() -> any CIFilter &amp; CIAccordionFoldTransition

Transitions by folding and crossfading an image to reveal the target image.

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

class func swipeTransition() -> any CIFilter &amp; CISwipeTransition

Gradually transitions from one image to another with a swiping motion.

