

- Core Image
- Transition Filters
-  modTransition() 

Type Method

# modTransition()

Transitions between two images by applying irregularly shaped holes.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func modTransition() -> any CIFilter & CIModTransition
```

## Return Value

The transition image.

## Discussion

This method applies the mod transition filter to an image. The effect transitions from the input image to the output image by revealing the target image through irregularly shaped holes.

The mod transition filter uses the following properties:

`inputImage`  
The starting image with the type CIImage.

`targetImage`  
The ending image with the type `CIImage`.

`center`  
A CGPoint representing the center of the image.

`angle`  
A `float` representing the angle of the effect as an NSNumber.

`radius`  
A `float` representing the size of the area of effect as an `NSNumber`.

`compression`  
A `float` representing the amount of stretching applied to the mod hole pattern as an `NSNumber`.

`time`  
A `float` representing the parametric time of the transition from start (at time 0) to end (at time 1) as an `NSNumber`.

The following code creates a filter that transitions from the input image to the target image by creating a series of irregular shaped holes.

func mod(inputImage: CIImage, targetImage: CIImage) -> CIImage {
    let modTransition = CIFilter.modTransition()
    modTransition.inputImage = inputImage
    modTransition.targetImage = targetImage
    modTransition.center = CGPoint(x: 390, y: 392)
    modTransition.time = 0.5
    modTransition.angle = 0.09
    modTransition.radius = 150
    modTransition.compression = 523   
    return modTransition.outputImage!
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

class func pageCurlTransition() -> any CIFilter &amp; CIPageCurlTransition

Simulates the curl of a page, revealing the target image.

class func pageCurlWithShadowTransition() -> any CIFilter &amp; CIPageCurlWithShadowTransition

Simulates the curl of a page, revealing the target image with added shadow.

class func rippleTransition() -> any CIFilter &amp; CIRippleTransition

Simulates a ripple in a pond to transiton from one image to another.

class func swipeTransition() -> any CIFilter &amp; CISwipeTransition

Gradually transitions from one image to another with a swiping motion.

