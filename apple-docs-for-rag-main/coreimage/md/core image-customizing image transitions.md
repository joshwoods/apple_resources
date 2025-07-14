

- Core Image
-  Customizing Image Transitions 

Article

# Customizing Image Transitions

Transition between images in creative ways using Core Image filters.

## Overview

You can add visual effects to an image transition by chaining together Core Image CIFilter objects in the category CICategoryTransition. Each filter from this category represents a single transition effect.

For example, you can combine an effect that dissolves an image and one that pixelates it as a transition to a second image. This particular transition chain comprises three steps:

1.  Create a dissolveTransition() transition filter with time as an input parameter.

2.  Create a pixellate() transition filter with time as an input parameter.

3.  Initiate the transition by adding a time step to your run loop.

Figure 1 Combine and to create a custom image transition.

### Load Source and Target Images

Filters in the transition category require your program to load both source and target images in order to transform the source into the destination.

let sourceURL = URL(fileURLWithPath: &quot;\(Bundle.main.bundlePath)/YourSourceImage.JPG&quot;)
let sourceCIImage = CIImage(contentsOf: sourceURL)

let destinationURL = URL(fileURLWithPath: &quot;\(Bundle.main.bundlePath)/YourTargetImage.JPG&quot;)
let destinationCIImage = CIImage(contentsOf: destinationURL)

### Create a Time-Dependent Dissolve Transition

The key difference of transition filters from their normal filter chain counterparts is the dependence on time. After creating a CIFilter from the Transition Filters category, you set the value of the `time` parameter to a float between `0.0` and `1.0` to indicate how far along the transition has progressed.

Write each transition filter to accept time as an input parameter, and reapply the filter at a regular interval to transform the image from its source state to the target state.

import simd

func dissolveFilter(_ inputImage: CIImage,
                    to targetImage: CIImage,
                    time: TimeInterval) -> CIImage? {
    let time = simd_smoothstep(0, 1, time)        
    let filter = CIFilter.dissolveTransition()
    filter.inputImage = inputImage
    filter.targetImage = targetImage
    filter.time = Float(time)
    return filter.outputImage
}

You don’t need to pass time linearly from `0.0` to `1.0`. In fact, you can advance the transition at a variable rate by modulating the time variable with a function, such as `simd_smoothstep`, which is a smooth ramp function clamped between two values, imbuing the dissolve effect with an ease-in ease-out feel.

Figure 2 simd_smoothstep(0, 1, time): a smooth ramp between 0 and 1

### Create a Time-Dependent Pixelate Transition

Like the dissolve transition, you can write the pixelate transition filter as a time-dependent function as well.

import simd

func pixelateFilter(_ inputImage: CIImage, time: TimeInterval) -> CIImage? {
    let scale = simd_smoothstep(1, 0, fabs(time))
    let filter = CIFilter.pixellate()
    filter.inputImage = inputImage
    filter.scale = 100 * Float(scale)
    return filter.outputImage
}

As with the dissolve filter, you can modify the speed and acceleration of the transition by changing the way time varies between `0.0` and `1.0`. In this case, unlike the `dissolveTransition()` filter, the `pixellate()` filter accepts a s`cale`, which you can vary over a smoothened triangle function: `simd_smoothstep(1, 0, abs(time))`.

Figure 3 simd_smoothstep(1, 0, abs(time)): a smoothened triangle ramp that goes from 0 to 1 to 0

This function puts the peak of the pixelation at the middle of the transition: the pixels start and end small, closely approximating the source image, but as the transition reaches its halfway point, the pixels scale to their largest size, effectively blocking out the moment farthest from source and target.

### Step Time with a Display Link

In writing the filter functions to accept a time parameter, you parametrized the transition effect moving from source to target. Now, you must move time forward when you want to perform the transition.

Adding a CADisplayLink to your run loop gives you a way to refresh an image every time a screen redraw occurs, so you can execute on a reliably regular time interval. In the case of a transition, you need only perform the following steps:

1.  Create the display link to call an update function.

2.  Add to your app’s main run loop to begin the transition. Start time at `0.0` and track time through the update function.

3.  In the update function, update the transition filters’ `inputTime` value and refresh the filtered image. Since this example chains two filters for a simultaneous effect, update both filters.

4.  In the update function, remove the link once time has expired.

Note

Adding a Timer may seem like a logical strategy for stepping time, but the display link fires with greater precision in sync with screen redraws.

#### Create the Display Link to Call an Update Function

displayLink = CADisplayLink(target: self, 
                            selector: #selector(stepTime))

Keeping the display link around beyond function scope allows you to remove it when the transition completes.

#### Add the Display Link to Begin the Transition

To begin the transition effect, add the CADisplayLink to your program’s main run loop, so it can execute each time step and redraw the transitioning CIImage.

func beginTransition() {

    time = 0
    dt = 0.005

    displayLink = CADisplayLink(target: self,
                                selector: #selector(stepTime))
    displayLink.add(to: RunLoop.current,
                    forMode: RunLoopMode.defaultRunLoopMode)
}

#### Write the Transition Update Function

The CADisplayLink should call a time-stepping function on each pass through the run loop. Inside this function, recompute the filtered image with that frame's `time` variable.

@objc
func stepTime() {

   time += dt

   // End transition after 1 second
   if time > 1 {
       displayLink.remove(from:RunLoop.main, forMode:RunLoopMode.defaultRunLoopMode)
   } else {
       guard let dissolvedCIImage = dissolveFilter(sourceCIImage,
                                                   to:finalCIImage,
                                                   time:time) else {
                                                      return
       }
       guard let pixelatedCIImage = pixelateFilter(dissolvedCIImage,
                                                   time:time) else {
                                                      return
       }
       // imageView and ciContext are properties of the class.
       showCIImage(pixelatedCIImage, in:imageView, context:ciContext)
   }
}

As a convenience, the following helper function shows a CIImage in a UIImageView.

func showCIImage(_ ciImage: CIImage,
                 in imageView: UIImageView,
                 context: CIContext) {

    guard let cgImage = context.createCGImage(ciImage,
                                              from: ciImage.extent) else {
                                                 return
    }
    let uiImage = UIImage(CGImage:cgImage)

    imageView.image = uiImage
}

### Explore Other Transition Visual Effects

The Core Image framework provides many distinct visual effects through its built-in catalog of filters. You can substitute a different transition effect for the dissolve and pixelation effects.

See filters under the Transition Filters collection for other effects to try.

For example, the copyMachineTransition() filter passes a scanning light over the source image as it transforms into the target image.

Figure 4 CICopyMachineTransition from a beach at sunset to a beach at daytime

The pageCurlWithShadowTransition() filter simulates the turn of a page, peeling the source image toward the right to reveal the target image underneath. You can include a separate image on the back of the flipped page.

Figure 5 CIPageCurlWithShadowTransition from a beach at daytime with rainbow in the sky to a beach at sunset, with a flower image on the back of the page

The barsSwipeTransition() slices the source image into vertical bars that sequentially slide off the page, revealing the target image underneath.

Figure 6 CIBarsSwipeTransition from a beach at sunset to a beach at daytime with rainbow in the sky

You can apply transitions such as accordion folding, flash photography, disintegration, and watery rippling. Substitute the dissolve and pixellate filters with others from the same category, and tweak the t`ime` or s`cale` parameter to customize the effect to fit your app.

## See Also

### Filter Recipes

Applying a Chroma Key Effect

Replace a color in one image with the background from another.

Selectively Focusing on an Image

Focus on a part of an image by applying Gaussian blur and gradient masks.

Simulating Scratchy Analog Film

Degrade the quality of an image to make it look like dated, analog film.

