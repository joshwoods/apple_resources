

- SwiftUI
- Image
-  Image.Scale 

Enumeration

# Image.Scale

A scale to apply to vector images relative to text.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Scale
```

## Overview

Use this type with the imageScale(_:) modifier, or the imageScale environment key, to set the image scale.

The following example shows the three `Scale` values as applied to a system symbol image, each set against a text view:

```
HStack { Image(systemName: "swift").imageScale(.small); Text("Small") }
HStack { Image(systemName: "swift").imageScale(.medium); Text("Medium") }
HStack { Image(systemName: "swift").imageScale(.large); Text("Large") }
```

## Topics

### Getting image scales

case small

A scale that produces small images.

case medium

A scale that produces medium-sized images.

case large

A scale that produces large images.

## Relationships

### Conforms To

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

enum Orientation

The orientation of an image.

enum ResizingMode

The modes that SwiftUI uses to resize an image to fit within its containing view.

