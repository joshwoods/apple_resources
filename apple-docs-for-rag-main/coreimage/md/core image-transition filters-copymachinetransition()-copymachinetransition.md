

- Core Image
- Transition Filters
-  copyMachineTransition() 

Type Method

# copyMachineTransition()

Simulates the effect of a copy machine scanner light to transiton between two images.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func copyMachineTransition() -> any CIFilter & CICopyMachineTransition
```

## Return Value

The transition image.

## Discussion

This method applies the copy machine transition filter to an image. The effect transitions from one image to another by simulating the scanning light effect of a copy machine.

The copy machine transition filter uses the following properties:

`inputImage`  
The starting image with the type CIImage.

`targetImage`  
The ending image with the type `CIImage`.

`time`  
A `float` representing the parametric time of the transition from start (at time 0) to end (at time 1) as an NSNumber.

`angle`  
A `float` representing the angle of the copier light, in radians as an `NSNumber`.

`width`  
A `float` representing the width of the effect as a `NSNumber`.

`extent`  
A CGRect representing the area of the copy machine effect.

`color`  
A CIColor representing the color of the light.

`opacity`  
A `float` representing the transparency of the copier light as an `NSNumber`.

The following code creates a filter that produces a light bar that glides across the input image revealing the target image:

func copyMachine(inputImage: CIImage, targetImage: CIImage) -> CIImage {
    let copyMachineTransition = CIFilter.copyMachineTransition()
    copyMachineTransition.inputImage = inputImage
    copyMachineTransition.targetImage = targetImage
    copyMachineTransition.time = 0.5
    copyMachineTransition.angle = 0.9
    copyMachineTransition.extent = CGRect(x: 54.1, y: 90.2, width: 300, height: 300)
    copyMachineTransition.color = .white
    copyMachineTransition.width = 200
    copyMachineTransition.opacity = 1.30   
    return copyMachineTransition.outputImage!
}

## See Also

### Filters

class func accordionFoldTransition() -> any CIFilter &amp; CIAccordionFoldTransition

Transitions by folding and crossfading an image to reveal the target image.

class func barsSwipeTransition() -> any CIFilter &amp; CIBarsSwipeTransition

Transitions between two images by removing rectangular portions of an image.

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

