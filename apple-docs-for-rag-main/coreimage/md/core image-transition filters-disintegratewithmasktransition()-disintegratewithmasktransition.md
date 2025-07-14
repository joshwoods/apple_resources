

- Core Image
- Transition Filters
-  disintegrateWithMaskTransition() 

Type Method

# disintegrateWithMaskTransition()

Transitions between two images using a mask image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func disintegrateWithMaskTransition() -> any CIFilter & CIDisintegrateWithMaskTransition
```

## Return Value

The transition image.

## Discussion

This method applies the disintegrate with mask transition filter to an image. The effect transitions from one image to another using the shapes defined by the mask image.

The disintegrate with mask transition filter uses the following properties:

`inputImage`  
The starting image with the type CIImage.

`targetImage`  
The ending image with the type `CIImage`.

`maskImage`  
An image with the type `CIImage`.

`time`  
A `float` representing the parametric time of the transition from start (at time 0) to end (at time 1) as an NSNumber.

`shadowRadius`  
A `float` representing the size of the shadow as a `NSNumber`.

`shadowDensity`  
A `float` representing the strength of the shadow as a `NSNumber`.

`shadowOffset`  
A CGPoint representing the size of the shadow from the mask image.

The following code creates a filter that produces a transition between the input and target images starting in the area’s outline in the mask image:

func disintergrate(inputImage: CIImage, targetImage: CIImage, maskImage: CIImage) -> CIImage {
    let disintergrateTransition  = CIFilter.disintegrateWithMaskTransition()
    disintergrateTransition.inputImage = inputImage
    disintergrateTransition.targetImage = targetImage
    disintergrateTransition.maskImage = maskImage
    disintergrateTransition.time = 0.5
    disintergrateTransition.shadowRadius = 8
    disintergrateTransition.shadowDensity = 0.65
    disintergrateTransition.shadowOffset = CGPoint(x: 0, y: -1)
    return disintergrateTransition.outputImage!
}

## See Also

### Filters

class func accordionFoldTransition() -> any CIFilter &amp; CIAccordionFoldTransition

Transitions by folding and crossfading an image to reveal the target image.

class func barsSwipeTransition() -> any CIFilter &amp; CIBarsSwipeTransition

Transitions between two images by removing rectangular portions of an image.

class func copyMachineTransition() -> any CIFilter &amp; CICopyMachineTransition

Simulates the effect of a copy machine scanner light to transiton between two images.

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

