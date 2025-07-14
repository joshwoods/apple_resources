

- Image I/O
-  CGImagePropertyOrientation 

Enumeration

# CGImagePropertyOrientation

A value describing the intended display orientation for an image.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum CGImagePropertyOrientation
```

## Overview

Values of this type define the position of the pixel coordinate origin point (`0,0`) and the directions of the coordinate axes relative to the intended display orientation of the image. Orientation values are commonly found in image metadata, and specifying image orientation correctly can be important both for displaying the image and for certain image processing tasks such as face recognition.

For example, the pixel data for an image captured by an iOS device camera is encoded in the camera sensor’s native landscape orientation. When the user captures a photo while holding the device in portrait orientation, iOS writes an orientation value of CGImagePropertyOrientation.right in the resulting image file. Software displaying the image can then, after reading that value from the file’s metadata, apply a 90° clockwise rotation to the image data so that the image appears in the photographer’s intended orientation.

### Compatibility with UIImageOrientation

The CGImagePropertyOrientation type covers the same set of orientation names available in from the UIImage.Orientation type, but the underlying numeric values of each type do not match. (For example, the “left mirrored” orientation has an underlying value of 5 in CGImagePropertyOrientation, but an underlying value of 7 in UIImage.Orientation.) If you have an orientation value in one type and need a semantically equivalent value in the other, use a function such as those below to produce the same-named value in the other type:

Listing 1. Converting between CGImagePropertyOrientation and UIImageOrientation

- Swift
- Objective-C

```
```

```
```

### Working with Raw TIFF/Exif Numeric Values

Some APIs describe image orientation with basic integer values, intended for interpretation according to the TIFF and Exif specifications. The CGImagePropertyOrientation type simply defines symbolic names for those values, so you can convert to and from the raw numeric type with C type-cast syntax or the inherited init(rawValue:) initializer and rawValue property in Swift.

## Topics

### Image Orientations

case up

The encoded image data matches the image’s intended display orientation.

case upMirrored

The encoded image data is horizontally flipped from the image’s intended display orientation.

case down

The encoded image data is rotated 180° from the image’s intended display orientation.

case downMirrored

The encoded image data is vertically flipped from the image’s intended display orientation.

case leftMirrored

The encoded image data is horizontally flipped and rotated 90° counter-clockwise from the image’s intended display orientation.

case right

The encoded image data is rotated 90° clockwise from the image’s intended display orientation.

case rightMirrored

The encoded image data is horizontally flipped and rotated 90° clockwise from the image’s intended display orientation.

case left

The encoded image data is rotated 90° clockwise from the image’s intended display orientation.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Image Information

let kCGImagePropertyImageCount: CFString

The number of images in the file.

let kCGImagePropertyIsIndexed: CFString

A Boolean value that indicates whether the image contains indexed pixel samples.

let kCGImagePropertyImages: CFString

An array of dictionaries, each of which contains metadata for one of the images in the file.

let kCGImagePropertyThumbnailImages: CFString

let kCGImagePropertyPrimaryImage: CFString

The index of the primary image in the file.

let kCGImagePropertyIsFloat: CFString

A Boolean value that indicates whether the image contains floating-point pixel samples.

let kCGImagePropertyOrientation: CFString

The intended display orientation of the image.

Individual Image Properties

Properties that apply to an individual image in an image source.

