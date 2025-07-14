

- AppKit
-  NSImageRep 

Class

# NSImageRep

A semiabstract superclass that provides subclasses that you use to draw an image from a particular type of source data.

macOS

``` source
class NSImageRep
```

## Overview

The NSImageRep class is called “semiabstract” because it has some instance variables and implementation of its own, in addition to defining subclasses. Although an NSImageRep subclass can be used directly, it is typically accessed through an NSImage object, which manages a group of image representations, choosing the best one for the current output device.

## Topics

### Creating Representations of Images

class func imageReps(withContentsOfFile: String) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the specified file.

class func imageReps(with: NSPasteboard) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the pasteboard.

class func imageReps(withContentsOf: URL) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the specified URL.

init?(contentsOfFile: String)

Creates and returns an image representation object using the contents of the specified file.

init?(pasteboard: NSPasteboard)

Creates and returns an image representation object using the contents of the specified pasteboard.

init?(contentsOf: URL)

Creates and returns an image representation object using the data at the specified URL.

init()

Creates and returns an image representation object.

init?(coder: NSCoder)

Creates and returns an image representation object from data in an unarchiver.

### Determining Types for Images

class func canInit(with: Data) -> Bool

Returns a Boolean value that indicates whether the image representation can initialize itself from the specified data.

class func canInit(with: NSPasteboard) -> Bool

Returns a Boolean value that indicates whether the receiver can initialize itself from the data on the specified pasteboard.

class var imageTypes: [String]

Returns an array of UTI strings identifying the image types supported by the image representation, either directly or through a user-installed filter service.

class var imageUnfilteredTypes: [String]

Returns an array of UTI strings identifying the image types supported directly by the ime representation.

class func imageFileTypes() -> [String]

Returns the file types supported by the image representation class or one of its subclasses.

Deprecated

class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns the pasteboard types supported by the image representation class or one of its subclasses.

Deprecated

class func imageUnfilteredFileTypes() -> [String]

Returns the list of file types supported directly by the image representation.

Deprecated

class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns the list of pasteboard types supported directly by the image representation.

Deprecated

### Accessing Size of Images

var size: NSSize

The size of the image representation, measured in points in the user coordinate space.

### Specifying Information About the Representation

var bitsPerSample: Int

The number of bits per sample in the object (if the object is a planar image, this property contains the number of bits per sample per plane).

var colorSpaceName: NSColorSpaceName

The name of the color space used by the image data.

var hasAlpha: Bool

A Boolean value that indicates whether the image data has an alpha channel.

var isOpaque: Bool

A Boolean value that indicates whether the image is opaque.

var pixelsHigh: Int

The height of the image, measured in pixels.

var pixelsWide: Int

The width of the image, measured in pixels.

var layoutDirection: NSImage.LayoutDirection

The layout direction for the image.

Device-Specific Value

A constant that is used by image representations to denote an attribute whose value changes to match the display device.

### Getting Core Graphics Images

func cgImage(forProposedRect: UnsafeMutablePointer&lt;NSRect>?, context: NSGraphicsContext?, hints: [NSImageRep.HintKey : Any]?) -> CGImage?

Returns a Core Graphics image object that captures the drawing of the image.

### Drawing Images

func draw() -> Bool

Implemented by subclasses to draw the image in the current coordinate system.

func draw(at: NSPoint) -> Bool

Draws the image representation’s image data at the specified point in the current coordinate system.

func draw(in: NSRect) -> Bool

Draws the image, scaling it (as needed) to fit the specified rectangle.

func draw(in: NSRect, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat, respectFlipped: Bool, hints: [NSImageRep.HintKey : Any]?) -> Bool

Draws all or part of the image in the specified rectangle in the current coordinate system.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

### Managing Representation Subclasses of Images

class func `class`(forType: String) -> AnyClass?

Returns the image representation subclass that handles image data for the specified UTI.

class func `class`(for: Data) -> AnyClass?

Returns the image representation subclass that handles the specified type of data.

class var registeredClasses: [AnyClass]

Returns an array containing the registered image representation classes.

class func registerClass(AnyClass)

Adds the specified class to the registry of available image representation subclasses.

class func unregisterClass(AnyClass)

Removes the specified image representation subclass from the registry of available image representations.

class func `class`(forFileType: String) -> AnyClass?

Returns the image representation subclass that handles data with the specified type.

Deprecated

class func `class`(forPasteboardType: NSPasteboard.PasteboardType) -> AnyClass?

Returns the image representation subclass that handles data with the specified pasteboard type.

Deprecated

### Notifications

class let registryDidChangeNotification: NSNotification.Name

Posted whenever the image representation class registry changes.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSBitmapImageRep
- NSCIImageRep
- NSCustomImageRep
- NSEPSImageRep
- NSPDFImageRep
- NSPICTImageRep

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

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

class NSImage

A high-level interface for manipulating image data.

protocol NSImageDelegate

A set of optional methods that you can use to respond to drawing failures and manage incremental loads.

