

- Core Image
-  Simulating Scratchy Analog Film 

Article

# Simulating Scratchy Analog Film

Degrade the quality of an image to make it look like dated, analog film.

## Overview

The sepiaTone() filter changes the tint of an image to a reddish-brownish hue resembling old analog photographs. You can enhance the effect by applying random specks and scratches.

Figure 1 Combine filtered white noise with dark scratches to the CISepiaTone filter to create an old analog film effect

The following steps leverage built-in Core Image filters to tint and texture an image to look as if it were analog film:

1.  Apply the `sepiaTone()` filter.

2.  Create randomly varying white specks to simulate grain.

3.  Create randomly varying dark scratches to simulate scratchy film.

4.  Composite the speckle image and scratches onto the sepia-toned image.

### Apply the Sepia Tone Filter to the Original Image

Tint the original image by applying the `sepiaTone()` filter.

let sepiaFilter = CIFilter.sepiaTone()
sepiaFilter.inputImage = inputImage
sepiaFilter.intensity = 1.0
let sepiaCIImage = sepiaFilter.outputImage

### Simulate Grain by Creating Randomly Varying Specks

You can use the output of the randomGenerator() filter to generate images containing random noise. Even though the noise pattern isn’t customizable in size, you can extend and crop it to fit the image.

Note

The image output from `randomGenerator()` is always the same; even if you reseed your random number generator, the image output from this filter is always the same 512x512 pattern. However, it’s suitable for giving the appearance of randomness. For truly random noise generation, see GameplayKit.

The filter takes no inputs.

let colorNoise = CIFilter.randomGenerator()
let noiseImage = colorNoise.outputImage

Next, apply a whitening effect by chaining the noise output to a colorMatrix() filter. This built-in filter multiplies the noise color values individually and applies a bias to each component. For white grain, apply whitening to the y-component of RGB and no bias.

let whitenVector = CIVector(x: 0, y: 1, z: 0, w: 0)
let fineGrain = CIVector(x:0, y:0.005, z:0, w:0)
let zeroVector = CIVector(x: 0, y: 0, z: 0, w: 0)
let whiteningFilter = CIFilter.colorMatrix()
whiteningFilter.inputImage = noiseImage
whiteningFilter.rVector = whitenVector
whiteningFilter.gVector = whitenVector
whiteningFilter.bVector = whitenVector
whiteningFilter.aVector = fineGrain
whiteningFilter.biasVector = zeroVector
let whiteSpecks = whiteningFilter.outputImage

The `whiteSpecks` resulting from this filter have the appearance of spotty grain when viewed as an image.

Figure 2 White speckle grain created from a whitening CIColorMatrix applied to CIRandomGenerator noise

Create the grainy image by compositing the whitened noise as input over the sepia-toned source image using the sourceOverCompositing() filter.

let speckCompositor = CIFilter.sourceOverCompositing()
speckCompositor.inputImage = whiteSpecks
speckCompositor.backgroundImage = sepiaCIImage
let speckledImage = speckCompositor.outputImage

### Simulate Scratch by Scaling Randomly Varying Noise

The process for applying random-looking scratches is the same as the technique used in the white grain: color the output of the `randomGenerator()` filter.

To make the speckle resemble scratches, scale the random noise output vertically by applying a scaling CGAffineTransform.

let verticalScale = CGAffineTransform(scaleX: 1.5, y: 25)
let transformedNoise = noiseImage.transformed(by: verticalScale)

Previously, you whitened the speckle image by applying the `CIColorMatrix` filter evenly across all color components. For the dark scratches, instead focus on only the red component, setting the other vector inputs to zero. This time, instead of multiplying the green, blue, and alpha channels, add bias `(0, 1, 1, 1)`.

let darkenVector = CIVector(x: 4, y: 0, z: 0, w: 0)
let darkenBias = CIVector(x: 0, y: 1, z: 1, w: 1)
let darkeningFilter = CIFilter.colorMatrix()
darkeningFilter.inputImage = noiseImage
darkeningFilter.rVector = darkenVector
darkeningFilter.gVector = zeroVector
darkeningFilter.bVector = zeroVector
darkeningFilter.aVector = zeroVector
darkeningFilter.biasVector = darkenBias
let randomScratches = darkeningFilter.outputImage.outputImage

The resulting scratches are cyan, so grayscale them using the minimumComponent() filter, which takes the minimum of the RGB values to produce a grayscale image.

let grayscaleFilter = CIFilter.minimumComponent()
grayscaleFilter.inputImage = randomScratches
let darkScratches = grayscaleFilter.outputImage

The grayscale filter produces random lines that resemble dark scratches.

Figure 3 Dark scratches created from a darkening CIColorMatrix applied to CIRandomGenerator noise

### Composite the Specks and Scratches to the Sepia Image

Now that the components are set, you can add the scratches to the grainy sepia image produced earlier. However, unlike the grainy texture, the scratches impact the image multiplicatively. Instead of the sourceOverCompositing() filter, which composites source over background, use the multiplyCompositing() filter to compose the scratches multiplicatively. Set the scratched image as the filter’s input image, and tab the speckle-composited sepia image as the input background image.

let oldFilmCompositor = CIFilter.multiplyCompositing()
oldFilmCompositor.inputImage = darkScratches
oldFilmCompositor.backgroundImage = speckledImage
let oldFilmImage = oldFilmCompositor.outputImage

Since the noise images had different dimensions than the source image, crop the composited result to the original image size to remove excess beyond the original extent.

let finalImage = oldFilmImage.cropped(to: inputImage.extent)

The cropped image represents the final result: a sepia-toned image with simulated grain and scratches composited to give it an analog film appearance.

Figure 4 Final result of CIMultiplyCompositing the source image with grain and scratches.

## See Also

### Filter Recipes

Applying a Chroma Key Effect

Replace a color in one image with the background from another.

Selectively Focusing on an Image

Focus on a part of an image by applying Gaussian blur and gradient masks.

Customizing Image Transitions

Transition between images in creative ways using Core Image filters.

