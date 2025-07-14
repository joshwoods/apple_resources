

- Image I/O
-  CGImageSource 

Class

# CGImageSource

An opaque type that you use to read image data from a URL, data object, or data consumer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CGImageSource
```

## Overview

Use a CGImageSource type to read data efficiently for most image file formats. The image source object manages the data buffers needed to load the image data and performs any operations on that data to turn it into a usable image. For example, it decompresses data stored in a compressed format. You can also use an image source to fetch or create thumbnail images and access metadata stored with the image.

Create an image source object from a CFURL, CFData, or CGDataProvider data type. The image source object reads data from the specified type and extracts the image information for you.

For more information, see Image I/O Programming Guide.

## Topics

### Creating an Image Source

func CGImageSourceCreateWithURL(CFURL, CFDictionary?) -> CGImageSource?

Creates an image source that reads from a location specified by a URL.

func CGImageSourceCreateWithData(CFData, CFDictionary?) -> CGImageSource?

Creates an image source that reads from a Core Foundation data object.

func CGImageSourceCreateWithDataProvider(CGDataProvider, CFDictionary?) -> CGImageSource?

Creates an image source that reads data from the specified data provider.

func CGImageSourceCreateIncremental(CFDictionary?) -> CGImageSource

Creates an empty image source that you can use to accumulate incremental image data.

### Extracting Images From an Image Source

func CGImageSourceCreateImageAtIndex(CGImageSource, Int, CFDictionary?) -> CGImage?

Creates an image object from the data at the specified index in an image source.

func CGImageSourceCreateThumbnailAtIndex(CGImageSource, Int, CFDictionary?) -> CGImage?

Creates a thumbnail version of the image at the specified index in an image source.

func CGImageSourceGetPrimaryImageIndex(CGImageSource) -> Int

Returns the index of the primary image for an High Efficiency Image File Format (HEIF) image.

### Getting Information From an Image Source

func CGImageSourceGetTypeID() -> CFTypeID

Returns the unique type identifier of an image source opaque type.

func CGImageSourceGetType(CGImageSource) -> CFString?

Returns the uniform type identifier of the source container.

func CGImageSourceCopyTypeIdentifiers() -> CFArray

Returns an array of uniform type identifiers that are supported for image sources.

func CGImageSourceGetCount(CGImageSource) -> Int

Returns the number of images (not including thumbnails) in the image source.

func CGImageSourceCopyProperties(CGImageSource, CFDictionary?) -> CFDictionary?

Returns the properties of the image source.

func CGImageSourceCopyPropertiesAtIndex(CGImageSource, Int, CFDictionary?) -> CFDictionary?

Returns the properties of the image at a specified location in an image source.

func CGImageSourceCopyAuxiliaryDataInfoAtIndex(CGImageSource, Int, CFString) -> CFDictionary?

Returns auxiliary data, such as mattes and depth information, that accompany the image.

### Updating an Incremental Image

func CGImageSourceUpdateData(CGImageSource, CFData, Bool)

Updates the data in an incremental image source.

func CGImageSourceUpdateDataProvider(CGImageSource, CGDataProvider, Bool)

Updates an incremental image source with a new data provider.

### Getting the Image Status

func CGImageSourceGetStatus(CGImageSource) -> CGImageSourceStatus

Return the status of an image source.

func CGImageSourceGetStatusAtIndex(CGImageSource, Int) -> CGImageSourceStatus

Returns the current status of an image at the specified location in the image source.

enum CGImageSourceStatus

The set of status values for images and image sources.

### Specifying the Read Options

let kCGImageSourceTypeIdentifierHint: CFString

The uniform type identifier that represents your best guess for the image’s type.

let kCGImageSourceShouldAllowFloat: CFString

A Boolean that indicates whether to use floating-point values in returned images.

let kCGImageSourceShouldCache: CFString

A Boolean value that indicates whether to cache the decoded image.

let kCGImageSourceShouldCacheImmediately: CFString

A Boolean value that indicates whether image decoding and caching happens at image creation time.

let kCGImageSourceCreateThumbnailFromImageIfAbsent: CFString

A Boolean value that indicates whether to create a thumbnail image automatically if the data source doesn’t contain one.

let kCGImageSourceCreateThumbnailFromImageAlways: CFString

A Boolean value that indicates whether to always create a thumbnail image.

let kCGImageSourceThumbnailMaxPixelSize: CFString

The maximum width and height of a thumbnail image, specified in pixels.

let kCGImageSourceCreateThumbnailWithTransform: CFString

A Boolean value that indicates whether to rotate and scale the thumbnail image to match the image’s orientation and aspect ratio.

let kCGImageSourceSubsampleFactor: CFString

The factor by which to scale down any returned images.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Image Management

class CGImageDestination

An opaque type that you use to write image data to a URL, data object, or data consumer.

