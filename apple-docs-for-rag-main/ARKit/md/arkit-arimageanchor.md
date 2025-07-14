

- ARKit
-  ARImageAnchor 

Class

# ARImageAnchor

An anchor for a known image that ARKit detects in the physical environment.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
class ARImageAnchor
```

## Overview

When you run a world-tracking AR session and specify ARReferenceImage objects for the session configuration’s detectionImages property, ARKit searches for those images in the real-world environment. When the session recognizes an image, it automatically adds an ARImageAnchor for each detected image to its list of anchors.

To find the extent of a recognized image in the scene, use the inherited transform property together with the physicalSize of the anchor’s referenceImage.

## Topics

### Identifying Detected Images

var referenceImage: ARReferenceImage

The detected image referenced by the image anchor.

### Estimating Scale

var estimatedScaleFactor: CGFloat

A factor between the initial size and the estimated physical size.

## Relationships

### Inherits From

- ARAnchor

### Conforms To

- ARAnchorCopying
- ARTrackable
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Image Detection

Tracking and altering images

Create images from rectangular shapes found in the user’s environment, and augment their appearance.

Detecting Images in an AR Experience

React to known 2D images in the user’s environment, and use their positions to place AR content.

class ARReferenceImage

A 2D image that you want ARKit to detect in the physical environment.

