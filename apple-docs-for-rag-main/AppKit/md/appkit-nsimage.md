

- AppKit
-  NSImage 

Class

# NSImage

A high-level interface for manipulating image data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
class NSImage
```

## Overview

You use instances of NSImage to load existing images, create new images, and draw the resulting image data into your views. Although you use this class predominantly for image-related operations, the class itself knows little about the underlying image data. Instead, it works in conjunction with one or more image representation objects (subclasses of NSImageRep) to manage and render the image data. For the most part, these interactions are transparent.

The class serves many purposes, providing support for the following tasks:

- Loading images stored on disk or at a specified URL.

- Drawing images into a view or graphics context.

- Providing the contents of a CALayer object.

- Creating new images based on a series of captured drawing commands.

- Producing versions of the image in a different format.

The `NSImage` class itself is capable of managing image data in a variety of formats. The specific list of formats is dependent on the version of the operating system but includes many standard formats such as TIFF, JPEG, GIF, PNG, and PDF among others. AppKit manages each format using a specific type of image representation object, whose job is to manage the actual image data. You can get a list of supported formats using the methods described in Determining Supported Types of Images.

For more information about how to use image objects in your app, see Cocoa Drawing Guide.

### Using Images with Core Animation Layers

Although you can assign an `NSImage` object directly to the contents property of a CALayer object, doing so may not always yield the best results. Instead of using your image object, you can use the layerContents(forContentsScale:) method to obtain an object that you can use for your layer’s contents. The image created by that method serves as the contents of a layer, which also supports all of the layer’s gravity modes. By contrast, the `NSImage` class supports only the resize, resizeAspect, and resizeAspectFill modes.

Before calling the layerContents(forContentsScale:) method, use the recommendedLayerContentsScale(_:) method to get the recommended scale factor for the resulting image. The code listing below shows a typical example that uses the scale factor of a window’s backing store as the desired scale factor. From that scale factor, the code gets the scale factor for the specified image object and creates an object that you assign to the layer. You might use this code for images that fit the layer bounds precisely or for which you rely on the contentsGravity property of the layer to position or scale the image.

Listing 1. Assigning an image to a layer

```
static void updateLayerWithImageInWindow1(NSImage *image, CALayer *layer, NSWindow *window) {
   CGFloat desiredScaleFactor = [window backingScaleFactor];
   CGFloat actualScaleFactor = [image recommendedLayerContentsScale:desiredScaleFactor];

   id layerContents = [image layerContentsForContentsScale:actualScaleFactor];

   [layer setContents:layerContents];
   [layer setContentsScale:actualScaleFactor];
}
```

## Topics

### Creating Images by Name

Configuring and displaying symbol images in your UI

Create scalable images that integrate with your app’s text, and adjust the appearance of those images dynamically.

init?(named: NSImage.Name)

Returns the image object associated with the specified name.

convenience init?(systemSymbolName: String, accessibilityDescription: String?)

Creates a symbol image with the system symbol name and accessibility description you specify.

convenience init?(systemSymbolName: String, variableValue: Double, accessibilityDescription: String?)

Creates a symbol image with the system symbol name and variable value you specify.

convenience init?(symbolName: String, variableValue: Double)

Creates a symbol image with the symbol name and variable value you specify.

convenience init?(symbolName: String, bundle: Bundle?, variableValue: Double)

convenience init(resource: ImageResource)

func setName(NSImage.Name?) -> Bool

Registers the image object under the specified name.

func name() -> NSImage.Name?

Returns the name associated with the image, if any.

typealias Name

Named images, defined by the system or you, for use in your app.

convenience init(imageLiteralResourceName: String)

Creates an image initialized with the specified resource name.

### Creating Dynamically Drawn Images

convenience init(size: NSSize, flipped: Bool, drawingHandler: (NSRect) -> Bool)

Creates and returns an image object whose contents are drawn using the specified block.

### Creating Images from Resource Files

convenience init?(byReferencingFile: String)

Initializes and returns an image object using the specified file.

convenience init(byReferencing: URL)

Initializes and returns an image object using the specified URL.

convenience init?(contentsOfFile: String)

Initializes and returns an image object with the contents of the specified file.

convenience init?(contentsOf: URL)

Initializes and returns an image object with the contents of the specified URL.

### Creating Images from Existing Data

convenience init?(data: Data)

Initializes and returns an image object using the provided image data.

convenience init?(dataIgnoringOrientation: Data)

Initializes and returns an image object using the provided image data and ignoring the EXIF orientation tags.

convenience init(cgImage: CGImage, size: NSSize)

Creates a new image using the contents of the provided image.

convenience init?(pasteboard: NSPasteboard)

Initializes and returns an image object with data from the specified pasteboard.

init(coder: NSCoder)

Initializes and returns an image object from data in an unarchiver.

### Creating Empty Images

init(size: NSSize)

Initializes and returns an image object with the specified dimensions.

### Creating Symbol Images

func withSymbolConfiguration(NSImage.SymbolConfiguration) -> NSImage?

Creates a new symbol image with the specified configuration.

class SymbolConfiguration

An object that contains the specific font, style, and weight attributes to apply to a symbol image.

### Getting the Symbol Image Configuration

var symbolConfiguration: NSImage.SymbolConfiguration

The configuration details for a symbol image.

### Managing Loading and Drawing of Images

var delegate: (any NSImageDelegate)?

The image’s delegate object.

protocol NSImageDelegate

A set of optional methods that you can use to respond to drawing failures and manage incremental loads.

### Setting Attributes of Images

var size: NSSize

The size of the image.

var isTemplate: Bool

A Boolean value that determines whether the image represents a template image.

var isTemplate: Bool

A Boolean value that determines whether the image represents a template image.

### Determining Supported Types of Images

class func canInit(with: NSPasteboard) -> Bool

Tests whether the image can create an instance of itself using pasteboard data.

class var imageTypes: [String]

Returns an array of UTI strings identifying the image types supported by the registered image representation objects, either directly or through a user-installed filter service.

class var imageUnfilteredTypes: [String]

Returns an array of UTI strings identifying the image types supported directly by the registered image representation objects.

### Working with Representations of Images

func addRepresentation(NSImageRep)

Adds the specified image representation object to the image.

func addRepresentations([NSImageRep])

Adds an array of image representation objects to the image.

var representations: [NSImageRep]

An array containing all of the image object’s image representations.

func removeRepresentation(NSImageRep)

Removes and releases the specified image representation.

func bestRepresentation(for: NSRect, context: NSGraphicsContext?, hints: [NSImageRep.HintKey : Any]?) -> NSImageRep?

Returns the best representation of the image for the specified rectangle using the provided hints.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

enum LayoutDirection

Constants that describe the layout direction for the image.

### Setting the Representation Selection Criteria for Images

var prefersColorMatch: Bool

A Boolean value that indicates whether the image prefers to choose image representations using color-matching or resolution-matching.

var usesEPSOnResolutionMismatch: Bool

A Boolean value that indicates whether EPS representations are preferred when no other representations match the resolution of the device.

var matchesOnMultipleResolution: Bool

A Boolean value that indicates whether image representations whose resolution is an integral multiple of the device resolution are a match.

### Drawing Images

func draw(in: NSRect)

Draws the image in the specified rectangle.

func draw(at: NSPoint, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat)

Draws all or part of the image at the specified point in the current coordinate system.

func draw(in: NSRect, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat)

Draws all or part of the image in the specified rectangle in the current coordinate system.

func draw(in: NSRect, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat, respectFlipped: Bool, hints: [NSImageRep.HintKey : Any]?)

Draws all or part of the image in the specified rectangle respecting the hints and the orientation of the current coordinate system.

func drawRepresentation(NSImageRep, in: NSRect) -> Bool

Draws the image using the specified image representation object.

enum NSCompositingOperation

Constants that describe compositing operators in terms of source and destination images, each having an opaque and transparent region.

### Managing Drawing Options

var isValid: Bool

A Boolean value that indicates whether it is possible to draw an image representation.

var backgroundColor: NSColor

The background color for the image.

var capInsets: NSEdgeInsets

The cap insets for the image.

var resizingMode: NSImage.ResizingMode

The resizing mode for the image.

enum ResizingMode

Constants that describe the resizing mode for the image.

### Working with Alignment Metadata

var alignmentRect: NSRect

A rectangle that you can use to position the image during layout.

### Managing Caching Options

var cacheMode: NSImage.CacheMode

The image’s caching mode.

func recache()

Invalidates and frees offscreen caches of all image representations.

enum CacheMode

Constants that specify the caching policy on a per-image basis.

### Producing TIFF Data for Images

var tiffRepresentation: Data?

A data object containing TIFF data for all of the image representations in the image.

func tiffRepresentation(using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a data object that contains TIFF data with the specified compression settings for all of the image representations in the image.

### Producing Core Graphics Images

func cgImage(forProposedRect: UnsafeMutablePointer&lt;NSRect>?, context: NSGraphicsContext?, hints: [NSImageRep.HintKey : Any]?) -> CGImage?

Returns a Core Graphics image based on the contents of the current image object.

### Hit-Testing Images

func hitTest(NSRect, withDestinationRect: NSRect, context: NSGraphicsContext?, hints: [NSImageRep.HintKey : Any]?, flipped: Bool) -> Bool

Returns whether the destination rectangle would intersect a non-transparent portion of the image.

### Managing Image Accessibility

var accessibilityDescription: String?

The image’s accessibility description.

### Using Images with Core Animation

func layerContents(forContentsScale: CGFloat) -> Any

Returns an object that may be used as the contents of a layer.

func recommendedLayerContentsScale(CGFloat) -> CGFloat

Returns the recommended layer contents scale for this image.

### Managing Axis Matching

var matchesOnlyOnBestFittingAxis: Bool

A Boolean value that indicates whether the image matches only on the best fitting axis.

### Localizing Images

func withLocale(Locale?) -> NSImage

var locale: Locale?

### Deprecated

Deprecated Symbols

Review symbols that are no longer supported, and find the replacements to use instead.

### Enumerations

enum DynamicRange

Describes how High Dynamic Range (HDR) image content displays.

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
- NSCoding
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSObjectProtocol
- NSPasteboardReading
- NSPasteboardWriting
- NSSecureCoding
- Transferable

## See Also

### Images

Providing images for different appearances

Supply image resources appropriate for light and dark appearances and for high-contrast environments.

Supporting Continuity Camera in Your Mac App

Incorporate scanned documents and pictures from a user’s iPhone, iPad, or iPod touch into your Mac app using Continuity Camera.

Supporting HDR images in your app

​Load, display, edit, and save HDR images using SwiftUI and Core Image. ​

Applying Apple HDR effect to your photos

You can decode and apply Apple’s HDR gain map to your own images.

protocol NSImageDelegate

A set of optional methods that you can use to respond to drawing failures and manage incremental loads.

class NSImageRep

A semiabstract superclass that provides subclasses that you use to draw an image from a particular type of source data.

