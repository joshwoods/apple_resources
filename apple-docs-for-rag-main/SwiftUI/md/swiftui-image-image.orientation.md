

- SwiftUI
- Image
-  Image.Orientation 

Enumeration

# Image.Orientation

The orientation of an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
enum Orientation
```

## Overview

Many image formats such as JPEG include orientation metadata in the image data. In other cases, you can specify image orientation in code. Properly specifying orientation is often important both for displaying the image and for certain kinds of image processing.

In SwiftUI, you provide an orientation value when initializing an Image from an existing CGImage.

## Topics

### Getting image orientations

case up

A value that indicates the original pixel data matches the image’s intended display orientation.

case down

A value that indicates a 180° rotation of the image from the orientation of its original pixel data.

case left

A value that indicates a 90° counterclockwise rotation from the orientation of its original pixel data.

case right

A value that indicates a 90° clockwise rotation of the image from the orientation of its original pixel data.

### Getting mirrored image orientation

case upMirrored

A value that indicates a horizontal flip of the image from the orientation of its original pixel data.

case downMirrored

A value that indicates a vertical flip of the image from the orientation of its original pixel data.

case leftMirrored

A value that indicates a 90° clockwise rotation and horizontal flip of the image from the orientation of its original pixel data.

case rightMirrored

A value that indicates a 90° counterclockwise rotation and horizontal flip from the orientation of its original pixel data.

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring an image

Fitting images into available space

Adjust the size and shape of images in your app’s user interface by applying view modifiers.

func imageScale(Image.Scale) -> some View

Scales images within the view according to one of the relative sizes available including small, medium, and large images sizes.

var imageScale: Image.Scale

The image scale for this environment.

enum Scale

A scale to apply to vector images relative to text.

enum ResizingMode

The modes that SwiftUI uses to resize an image to fit within its containing view.

