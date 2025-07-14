

- Core Image
-  Processing an Image Using Built-in Filters 

Article

# Processing an Image Using Built-in Filters

Apply effects such as sepia tint, highlight strengthening, and scaling to images.

## Overview

You can add effects to images by applying Core Image filters to CIImage objects. Figure 1 shows three filters chained together to achieve a cumulative effect:

1.  Apply the sepia filter to tint an image with a reddish-brown hue.

2.  Add the bloom filter to accentuate highlights.

3.  Use the Lanczos scale filter to scale an image down.

Figure 1 Filtering a waterwheel image using built-in Core Image filters

### Create a Context

CIImage processing occurs in a CIContext object. Creating a CIContext is expensive, so create one during your initial setup and reuse it throughout your app.

let context = CIContext()

Listing 1 Creating a context in Core Image

### Load an Image to Process

The next step is to load an image to process. This example loads an image from the project bundle.

let imageURL = URL(fileURLWithPath: &quot;\(Bundle.main.bundlePath)/YourImageName.png&quot;)
let originalCIImage = CIImage(contentsOf: imageURL)!
self.imageView.image = UIImage(ciImage:originalCIImage)

Listing 2 Loading an image into CIImage

The CIImage object isn’t itself a displayable image, but rather image data. To display it, you must convert it to another type, such as UIImage.

### Apply Built-In Core Image Filters

A CIFilter represents a single operation or recipe for a particular effect. To process a CIImage object, pass it through CIFilter objects. You can subclass CIFilter or draw from the existing library of built-in filters.

#### Tint Reddish-Brown with the Sepia Filter

Although you can chain filters without separating them into functions, the following example shows how to configure a single CIFilter, the sepiaTone() filter.

func sepiaFilter(_ input: CIImage, intensity: Float) -> CIImage? {
    let sepiaFilter = CIFilter.sepiaTone()
    sepiaFilter.inputImage = input
    sepiaFilter.intensity = intensity
    return sepiaFilter.outputImage
}

Listing 3 Applying sepia tint as a

To pass the image through the filter, call the sepia filter function.

let sepiaCIImage = sepiaFilter(originalCIImage, intensity:0.9)

Listing 4 Calling the sepia filter function

You can check the intermediate result at any point in the filter chain by converting from CIImage to a UIImage. You can then assign this `UIImage` to a UIImageView for display.

self.imageView.image = UIImage(ciImage:sepiaCIImage!)

Listing 5 Displaying intermediate outputs as

#### Strengthen Highlights with the Bloom Filter

The bloom filter accentuates the highlights of an image. You can apply it as part of a chain without factoring it into a separate function, but this example encapsulates its functionality into a function.

func bloomFilter(_ input:CIImage, intensity: Float, radius: Float) -> CIImage? {
    let bloomFilter = CIFilter.bloom()
    bloomFilter.inputImage = input
    bloomFilter.intensity = intensity
    bloomFilter.radius
    return bloomFilter.outputImage
}

Listing 6 Applying the bloom filter as a

Like the sepia filter, the intensity of the bloom filter’s effect ranges between 0 and 1, with 1 being the most intense effect. The bloom filter has an additional r`adius` parameter to determine how much the glowing regions expand. Experiment with a range to values to fine tune the effect, or assign the input parameter to a control like a UISlider to allow your users to tweak its values.

Note

The gloom() filter performs the opposite effect.

To display the output, convert the CIImage to a UIImage.

let bloomCIImage = bloomFilter(sepiaCIImage, intensity:1, radius:10)
_imageView.image = UIImage(ciImage:bloomCIImage)

Listing 7 Calling the bloom filter

#### Scale Image Size with the Lanczos Scale Filter

Apply the lanczosScaleTransform() to obtain a high-quality downsampling of the image, preserving the original image’s aspect ratio through the `lanczosScaleTransform()` filter’s parameter `aspectRatio`. For built-in Core Image filters, calculate the aspect ratio as the image’s width over height, as in Listing 8.

CGFloat imageWidth = originalUIImage.size.width
CGFloat imageHeight = originalUIImage.size.height
let aspectRatio = Double(originalImage.size.width) / Double(originalImage.size.height)
let scaledCIImage = scaleFilter(bloomCIImage, aspectRatio:aspectRatio, scale:0.5)

Listing 8 Computing aspect ratio as height over width

Like other built-in filters, the lanczosScaleTransform() filter also outputs its result as a CIImage.

func scaleFilter(_ input:CIImage, aspectRatio : Float, scale : Float) -> CIImage {
    let scaleFilter = CIFilter.lanczosScaleTransform()
    scaleFilter.inputImage = input
    scaleFilter.scale = scale
    scaleFilter.aspectRatio = aspectRatio
    return scaleFilter.outputImage!
}

Listing 9 Applying the Lanczos scale transform as a

Important

To optimize computation, Core Image doesn’t actually render any intermediate CIImage result until you force the CIImage to display its content onscreen, as you might do using UIImageView.

self.imageView.image = UIImage(ciImage:scaledCIImage)

Listing 10 Showing the final result in a

Note

Core Image optimizes filtering by reordering the three chained filters and concatenating them into a single image processing kernel, saving computation and rendering cycles.

In addition to trying out the built-in filters for a fixed effect, you can combine filters in certain Filter Recipes to accomplish tasks such as Applying a Chroma Key Effect, Selectively Focusing on an Image, Customizing Image Transitions, and Simulating Scratchy Analog Film.

## See Also

### Essentials

class CIContext

An evaluation context for rendering image processing results and performing image analysis.

class CIImage

A representation of an image to be processed or produced by Core Image filters.

