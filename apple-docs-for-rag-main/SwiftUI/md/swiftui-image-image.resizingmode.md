

- SwiftUI
- Image
-  Image.ResizingMode 

Enumeration

# Image.ResizingMode

The modes that SwiftUI uses to resize an image to fit within its containing view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum ResizingMode
```

## Topics

### Getting resizing modes

case stretch

A mode to enlarge or reduce the size of an image so that it fills the available space.

case tile

A mode to repeat the image at its original size, as many times as necessary to fill the available space.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
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

enum Orientation

The orientation of an image.

