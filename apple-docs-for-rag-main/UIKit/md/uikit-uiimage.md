

- UIKit
-  UIImage 

Class

# UIImage

An object that manages image data in your app.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class UIImage
```

## Mentioned in 

Configuring and displaying symbol images in your UI

Making a view into a drop destination

Understanding a drag item as a promise

## Overview

You use image objects to represent image data of all kinds, and the UIImage class is capable of managing data for all image formats supported by the underlying platform. Image objects are immutable, so you always create them from existing image data, such as an image file on disk or programmatically created image data. An image object may contain a single image or a sequence of images for use in an animation.

You can use image objects in several different ways:

- Assign an image to a UIImageView object to display the image in your interface.

- Use an image to customize system controls such as buttons, sliders, and segmented controls.

- Draw an image directly into a view or other graphics context.

- Pass an image to other APIs that might require image data.

Although image objects support all platform-native image formats, it’s recommended that you use PNG or JPEG files for most images in your app. Image objects are optimized for reading and displaying both formats, and those formats offer better performance than most other image formats. Because the PNG format is lossless, it’s especially recommended for the images you use in your app’s interface.

### Create image objects

When creating image objects using the methods of this class, you must have existing image data located in a file or data structure. You can’t create an empty image and draw content into it. There are many options for creating image objects, each of which is best for specific situations:

- Use the init(named:in:compatibleWith:) method (or the init(named:) method) to create an image from an image asset or image file located in your app’s main bundle (or some other known bundle). Because these methods cache the image data automatically, they’re especially recommended for images that you use frequently.

- Use the imageWithContentsOfFile: or init(contentsOfFile:) method to create an image object where the initial data isn’t in a bundle. These methods load the image data from disk each time, so don’t use them to load the same image repeatedly.

- Use the animatedImage(with:duration:) and animatedImageNamed(_:duration:) methods to create a single UIImage object comprised of multiple sequential images. Install the resulting image in a UIImageView object to create animations in your interface.

Other methods of the UIImage class let you create animations from specific types of data, such as Core Graphics images or image data you create yourself. UIKit also provides the UIGraphicsGetImageFromCurrentImageContext() function to create images from content you draw yourself. You use that function in conjunction with a bitmap-based graphics context, which you use to capture your drawing commands.

Note

Because image objects are immutable, you can’t change their properties after creation. Most image properties are set automatically using metadata in the accompanying image file or image data. The immutable nature of image objects also means they’re safe to create and use from any thread.

Image assets are the easiest way to manage the images that ship with your app. Each new Xcode project contains an assets library, to which you can add multiple image sets. An image set contains the variations of a single image that your app uses. A single image set can provide different versions of an image for different platforms, for different trait environments (compact or regular), and for different scale factors.

In addition to loading images from disk, you can ask the user to supply images from an available camera or photo library using a UIImagePickerController object. An image picker displays a custom user interface for selecting images. Accessing user-supplied images requires explicit user permission. For more information about using an image picker, see UIImagePickerController.

### Define a stretchable image

A stretchable image is one that defines regions where you can duplicate the underlying image data in an aesthetically pleasing way. Stretchable images are commonly used to create backgrounds that can grow or shrink to fill the available space.

Define a stretchable image by adding insets to an existing image using the resizableImage(withCapInsets:) or resizableImage(withCapInsets:resizingMode:) method. The insets subdivide the image into two or more parts. Specifying nonzero values for each inset yields an image divided into nine parts, as shown in the following image:

Each inset defines the portion of the image that doesn’t stretch in the given dimension. The regions inside an image’s top and bottom insets maintain a fixed height, and the areas inside the left and right insets maintain a fixed width. The following image shows how each part of a nine-part image stretches as the image itself is stretched to fill the available space. The corners of the image don’t change size because they’re inside both a horizontal and vertical inset:

### Compare images

The isEqual(_:) method is the only reliable way to determine whether two image objects contain the same image data. The following code illustrates the correct and incorrect ways to compare images.

- Swift
- Objective-C

```
// Load the same image twice.
let image1 = UIImage(named: "MyImage")
let image2 = UIImage(named: "MyImage") 

// The image objects may be different, but the contents are still equal.
if image1 != nil && image1!.isEqual(image2) {
    // Correct. This technique compares the image data correctly.
} 
if image1 == image2 {
    // Incorrect! Direct object comparisons may not work.
}
```

```
// Load the same image twice.
UIImage* image1 = [UIImage imageNamed:@"MyImage"];
UIImage* image2 = [UIImage imageNamed:@"MyImage"];

// The image objects may be different, but the contents are still equal
if ([image1 isEqual:image2]) {
   // Correct. This technique compares the image data correctly.
}

if (image1 == image2) {
   // Incorrect! Direct object comparisons may not work.
}
```

### Access the image data

Image objects don’t provide direct access to their underlying image data. However, you can retrieve the image data in other formats for use in your app. Specifically, you can use the cgImage and ciImage properties to retrieve versions of the image that are compatible with Core Graphics and Core Image, respectively. You can also use the pngData() and jpegData(compressionQuality:) functions to generate an NSData object containing the image data in either the PNG or JPEG format.

## Topics

### Loading and caching images

Providing images for different appearances

Supply image resources appropriate for light and dark appearances and for high-contrast environments.

Configuring and displaying symbol images in your UI

Create scalable images that integrate with your app’s text, and adjust the appearance of those images dynamically.

Creating custom symbol images for your app

Create, organize, and annotate symbol images using SF Symbols.

init?(named: String, in: Bundle?, compatibleWith: UITraitCollection?)

Creates an image object using the named image asset that’s compatible with the specified trait collection.

init?(named: String, in: Bundle?, with: UIImage.Configuration?)

Creates an image by using the named image asset that’s compatible with the configuration you specify.

convenience init?(named: String, in: Bundle?, variableValue: Double, configuration: UIImage.Configuration?)

Creates an image by using the name, configuration, and variable value you specify.

init?(named: String)

Creates an image object from the specified named asset.

convenience init(imageLiteralResourceName: String)

Returns the image object for the specified resource.

init?(systemName: String, withConfiguration: UIImage.Configuration?)

Creates an image object that contains a system symbol image with the specified configuration.

convenience init?(systemName: String, variableValue: Double, configuration: UIImage.Configuration?)

Creates an image object that contains a system symbol image with the configuration and variable value you specify.

init?(systemName: String, compatibleWith: UITraitCollection?)

Creates an image object that contains a system symbol image appropriate for the specified traits.

init?(systemName: String)

Creates an image object that contains a system symbol image.

convenience init(resource: ImageResource)

Building high-performance lists and collection views

Improve the performance of lists and collections in your app with prefetching and image preparation.

### Loading images for display

func preparingForDisplay() -> UIImage?

Decodes an image synchronously and provides a new one for display in views and animations.

func prepareForDisplay(completionHandler: (UIImage?) -> Void)

Decodes an image asynchronously and provides a new one for display in views and animations.

func preparingThumbnail(of: CGSize) -> UIImage?

Returns a new thumbnail image at the specified size.

func prepareThumbnail(of: CGSize, completionHandler: (UIImage?) -> Void)

Creates a thumbnail image at the specified size asynchronously on a background thread.

### Creating and initializing image objects

init?(contentsOfFile: String)

Initializes and returns the image object with the contents of the specified file.

init?(data: Data)

Initializes and returns the image object with the specified data.

init?(data: Data, scale: CGFloat)

Initializes and returns the image object with the specified data and scale factor.

init(cgImage: CGImage)

Initializes and returns the image object with the specified Quartz image reference.

init(cgImage: CGImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified scale and orientation factors.

init(ciImage: CIImage)

Initializes and returns an image object with the specified Core Image object.

init(ciImage: CIImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified Core Image object and properties.

struct UIImageReader

### Creating animated images

class func animatedImageNamed(String, duration: TimeInterval) -> UIImage?

Creates and returns an animated image.

class func animatedImage(with: [UIImage], duration: TimeInterval) -> UIImage?

Creates and returns an animated image from an existing set of images.

class func animatedResizableImageNamed(String, capInsets: UIEdgeInsets, duration: TimeInterval) -> UIImage?

Creates and returns an animated image with end caps.

class func animatedResizableImageNamed(String, capInsets: UIEdgeInsets, resizingMode: UIImage.ResizingMode, duration: TimeInterval) -> UIImage?

Creates and returns an animated image with end caps and a specific resizing mode.

### Changing the image attributes

func withConfiguration(UIImage.Configuration) -> UIImage

Returns a new version of the current image, replacing the current configuration attributes with the specified attributes.

func applyingSymbolConfiguration(UIImage.SymbolConfiguration) -> UIImage?

Returns a new version of the current image, applying the specified configuration attributes on top of the current attributes.

func imageFlippedForRightToLeftLayoutDirection() -> UIImage

Returns a new version of the current image that flips horizontally when it’s in a right-to-left layout.

func withHorizontallyFlippedOrientation() -> UIImage

Returns a new version of the image that’s a mirror of the original image.

func withRenderingMode(UIImage.RenderingMode) -> UIImage

Returns a new version of the image that uses the specified rendering mode.

func withAlignmentRectInsets(UIEdgeInsets) -> UIImage

Returns a new version of the image that uses the specified alignment insets.

func resizableImage(withCapInsets: UIEdgeInsets) -> UIImage

Returns a new version of the image with the specified cap insets.

func resizableImage(withCapInsets: UIEdgeInsets, resizingMode: UIImage.ResizingMode) -> UIImage

Returns a new version of the image with the specified cap insets and options.

func imageWithoutBaseline() -> UIImage

Creates a copy of the current image object without any baseline information.

func withBaselineOffset(fromBottom: CGFloat) -> UIImage

Creates a new image with a baseline at the specified offset from the bottom of the image.

class Configuration

A configuration object that contains the traits that the system uses when selecting the current image variant.

class SymbolConfiguration

An object that contains the specific font, size, style, and weight attributes to apply to a symbol image.

### Getting standard system images

class var add: UIImage

The standard image for indicating the addition of content.

class var remove: UIImage

The standard image for indicating the removal of content.

class var actions: UIImage

The standard image for indicating user-initiated actions.

class var checkmark: UIImage

The standard image for a checkmark on a filled-circle background.

class var strokedCheckmark: UIImage

The standard image for a checkmark on a tinted circle with a white-stroked border.

### Getting the image data

var cgImage: CGImage?

The underlying Quartz image data.

var ciImage: CIImage?

The underlying Core Image data.

var images: [UIImage]?

The complete array of image objects that compose the animation of an animated object.

var imageAsset: UIImageAsset?

The image asset (if any) for the image.

### Getting the image size and scale

var scale: CGFloat

The scale factor of the image.

var size: CGSize

The logical dimensions, in points, for the image.

### Accessing image attributes

var imageOrientation: UIImage.Orientation

The orientation of the receiver’s image.

enum Orientation

Constants that specify the intended display orientation for an image.

var flipsForRightToLeftLayoutDirection: Bool

A Boolean value that indicates whether the image flips in a right-to-left layout.

var resizingMode: UIImage.ResizingMode

The resizing mode of the image.

enum ResizingMode

Constants that specify the possible resizing modes for an image.

var duration: TimeInterval

The time interval for displaying an animated image.

var capInsets: UIEdgeInsets

The end-cap insets.

var alignmentRectInsets: UIEdgeInsets

The alignment metadata for positioning the image during layout.

var isSymbolImage: Bool

A Boolean value that indicates whether the image is a symbol.

### Getting the image configuration

var configuration: UIImage.Configuration?

The configuration details for the image.

var symbolConfiguration: UIImage.SymbolConfiguration?

The configuration details for a symbol image.

var traitCollection: UITraitCollection

The trait collection that describes the current variant of the image.

### Specifying the dynamic range

var isHighDynamicRange: Bool

func imageRestrictedToStandardDynamicRange() -> UIImage

func heicData() -> Data?

enum DynamicRange

### Managing the baseline

var baselineOffsetFromBottom: CGFloat?

The position of the baseline relative to the bottom of the image.

### Getting rendering information

var renderingMode: UIImage.RenderingMode

A setting that determines how the app renders an image.

enum RenderingMode

Constants that specify the possible rendering modes for an image.

var imageRendererFormat: UIGraphicsImageRendererFormat

The preferred image renderer format for the image.

### Tinting the image

func withTintColor(UIColor) -> UIImage

Returns a new version of the current image with the specified tint color.

func withTintColor(UIColor, renderingMode: UIImage.RenderingMode) -> UIImage

Returns a new version of the image with a tint color that uses the specified rendering mode.

### Drawing images

func draw(at: CGPoint)

Draws the image at the specified point in the current context.

func draw(at: CGPoint, blendMode: CGBlendMode, alpha: CGFloat)

Draws the entire image at the specified point using the custom compositing options.

func draw(in: CGRect)

Draws the entire image in the specified rectangle, scaling it as necessary to fit.

func draw(in: CGRect, blendMode: CGBlendMode, alpha: CGFloat)

Draws the entire image in the specified rectangle using the specified compositing options.

func drawAsPattern(in: CGRect)

Draws a tiled Quartz pattern using the receiver’s contents as the tile pattern.

### Exporting standard bitmap formats

func jpegData(compressionQuality: CGFloat) -> Data?

Returns a data object that contains the image in JPEG format.

func pngData() -> Data?

Returns a data object that contains the specified image in PNG format.

### Deprecated

func stretchableImage(withLeftCapWidth: Int, topCapHeight: Int) -> UIImage

Creates and returns a new image object with the specified cap values.

Deprecated

var leftCapWidth: Int

The horizontal end-cap size.

Deprecated

var topCapHeight: Int

The vertical end-cap size.

Deprecated

### Default Implementations

JournalingSuggestionAsset Implementations

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- JournalingSuggestionAsset
- NSCoding
- NSItemProviderReading
- NSItemProviderWriting
- NSObjectProtocol
- NSSecureCoding
- Sendable
- UIAccessibilityIdentification
- UIItemProviderPresentationSizeProviding

## See Also

### Representations

class SymbolConfiguration

An object that contains the specific font, size, style, and weight attributes to apply to a symbol image.

class Configuration

A configuration object that contains the traits that the system uses when selecting the current image variant.

