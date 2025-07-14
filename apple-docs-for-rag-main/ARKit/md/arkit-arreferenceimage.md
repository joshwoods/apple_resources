

- ARKit
-  ARReferenceImage 

Class

# ARReferenceImage

A 2D image that you want ARKit to detect in the physical environment.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
class ARReferenceImage
```

## Overview

To accurately detect the position and orientation of a 2D image in the real world, ARKit requires preprocessed image data and knowledge of the image’s real-world dimensions. The ARReferenceImage class encapsulates this information. To enable image detection in an AR session, pass a collection of reference images to your session configuration’s detectionImages property.

Typically, you create reference images in your Xcode project’s asset catalog:

1.  In your asset catalog, use the Add (+) button to create an AR Resource Group.

2.  Drag image files into the resource group to create AR Reference Image entries in the asset catalog.

3.  For each reference image, use the Xcode inspector panel to provide the real-world size at which you want ARKit to recognize the image. (You can also provide a descriptive name, which appears as the name property at runtime and can be useful for debugging.)

## Topics

### Loading Reference Images

class func referenceImages(inGroupNamed: String, bundle: Bundle?) -> Set&lt;ARReferenceImage>?

Loads all reference images in the specified AR Resource Group in your Xcode project’s asset catalog.

### Examining a Reference Image

var name: String?

A descriptive name for the image.

var physicalSize: CGSize

The real-world dimensions, in meters, of the image.

var resourceGroupName: String?

The AR resource group name for this image.

### Creating Reference Images

init(CGImage, orientation: CGImagePropertyOrientation, physicalWidth: CGFloat)

Creates a new reference image from a Core Graphics image object.

init(CVPixelBuffer, orientation: CGImagePropertyOrientation, physicalWidth: CGFloat)

Creates a new reference image from a Core Video pixel buffer.

### Validating Reference Images

func validate(completionHandler: ((any Error)?) -> Void)

Determines whether the reference image is valid.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Image Detection

Tracking and altering images

Create images from rectangular shapes found in the user’s environment, and augment their appearance.

Detecting Images in an AR Experience

React to known 2D images in the user’s environment, and use their positions to place AR content.

class ARImageAnchor

An anchor for a known image that ARKit detects in the physical environment.

