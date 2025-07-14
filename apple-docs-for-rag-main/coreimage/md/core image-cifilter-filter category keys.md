

- Core Image
- CIFilter
-  Filter Category Keys 

API Collection

# Filter Category Keys

Categories of filters.

## Topics

### Constants

let kCICategoryDistortionEffect: String

A filter that reshapes an image by altering its geometry to create a 3D effect. Using distortion filters, you can displace portions of an image, apply lens effects, make a bulge in an image, and perform other operation to achieve an artistic effect.

let kCICategoryGeometryAdjustment: String

A filter that changes the geometry of an image. Some of these filters are used to warp an image to achieve an artistic effects, but these filters can also be used to correct problems in the source image. For example, you can apply an affine transform to straighten an image that is rotated with respect to the horizon.

let kCICategoryCompositeOperation: String

A filter operates on two image sources, using the color values of one image to operate on the other. Composite filters perform computations such as computing maximum values, minimum values, and multiplying values between input images. You can use compositing filters to add effects to an image, crop an image, and achieve a variety of other effects.

let kCICategoryHalftoneEffect: String

A filter that simulates a variety of halftone screens, to mimic the halftone process used in print media. The output of these filters has the familiar “newspaper” look of the various dot patterns. Filters are typically named after the pattern created by the virtual halftone screen, such as circular screen or hatched screen.

let kCICategoryColorAdjustment: String

A filter that changes color values. Color adjustment filters are used to eliminate color casts, adjust hue, and correct brightness and contrast. Color adjustment filters do not perform color management; ColorSync performs color management. You can use Quartz 2D to specify the color space associated with an image. For more information, see Color Management Overview and Quartz 2D Programming Guide.

let kCICategoryColorEffect: String

A filter that modifies the color of an image to achieve an artistic effect. Examples of color effect filters include filters that change a color image to a sepia image or a monochrome image or that produces such effects as posterizing.

let kCICategoryTransition: String

A filter that provides a bridge between two or more images by applying a motion effect that defines how the pixels of a source image yield to that of the destination image.

let kCICategoryTileEffect: String

A filter that typically applies an effect to an image and then create smaller versions of the image (tiles), which are then laid out to create a pattern that’s infinite in extent.

let kCICategoryGenerator: String

A filter that generates a pattern, such as a solid color, a checkerboard, or a star shine. The generated output is typically used as input to another filter.

let kCICategoryReduction: String

A filter that reduces image data. These filters are used to solve image analysis problems.

let kCICategoryGradient: String

A filter that generates a fill whose color varies smoothly. Exactly how color varies depends on the type of gradient—linear, radial, or Gaussian.

let kCICategoryStylize: String

A filter that makes a photographic image look as if it was painted or sketched. These filters are typically used alone or in combination with other filters to achieve artistic effects.

let kCICategorySharpen: String

A filter that sharpens images, increasing the contrast between the edges in an image. Examples of sharpen filters are unsharp mask and sharpen luminance.

let kCICategoryBlur: String

A filter that softens images, decreasing the contrast between the edges in an image. Examples of blur filters are Gaussian blur and zoom blur.

let kCICategoryVideo: String

A filter that works on video images.

let kCICategoryStillImage: String

A filter that works on still images.

let kCICategoryInterlaced: String

A filter that works on interlaced images.

let kCICategoryNonSquarePixels: String

A filter that works on non-square pixels.

let kCICategoryHighDynamicRange: String

A filter that works on high dynamic range pixels.

let kCICategoryBuiltIn: String

A filter provided by Core Image. This distinguishes built-in filters from plug-in filters.

let kCICategoryFilterGenerator: String

A filter created by chaining several filters together and then packaged as a CIFilterGenerator object.

