

- Core Image
- Transition Filters
-  pageCurlTransition() 

Type Method

# pageCurlTransition()

Simulates the curl of a page, revealing the target image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func pageCurlTransition() -> any CIFilter & CIPageCurlTransition
```

## Return Value

The transition image.

## Discussion

This method applies the page curl transition filter to an image. The effect transitions from one image to another by simulating a curling page, revealing the target image as the page curls.

The page curl transition filter uses the following properties:

`inputImage `  
The starting image with the type CIImage.

`targetImage`  
The ending image with the type `CIImage`.

`backsideImage`  
An image used as the backside of the curl with the type `CIImage`.

`extent`  
A CGRect representing the size of the effect.

`time`  
A `float` representing the parametric time of the transition from start (at time 0) to end (at time 1) as an NSNumber.

`angle`  
A `float` representing the angle of the motion of the curl as an `NSNumber`.

`radius`  
A `float` representing the radius of the curl as an `NSNumber`.

The following code creates a filter that produces a page curling back to reveal the target image.

func pageCurl(inputImage: CIImage, targetImage: CIImage, backsideImage: CIImage) -> CIImage {
    let pageCurlTransition = CIFilter.pageCurlTransition()
    pageCurlTransition.inputImage = inputImage
    pageCurlTransition.targetImage = targetImage
    pageCurlTransition.backsideImage = backsideImage
    pageCurlTransition.extent = CGRect(x: 54, y: 90, width: 300, height: 300)
    pageCurlTransition.time = 5.6
    pageCurlTransition.angle = 0.9
    pageCurlTransition.radius = 150
    return pageCurlTransition.outputImage!
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

class func pageCurlWithShadowTransition() -> any CIFilter &amp; CIPageCurlWithShadowTransition

Simulates the curl of a page, revealing the target image with added shadow.

class func rippleTransition() -> any CIFilter &amp; CIRippleTransition

Simulates a ripple in a pond to transiton from one image to another.

class func swipeTransition() -> any CIFilter &amp; CISwipeTransition

Gradually transitions from one image to another with a swiping motion.

