

- ClockKit
-  CLKFullColorImageProvider Deprecated

Class

# CLKFullColorImageProvider

A full-color image displayed by a complication.

watchOS 5.0–9.0Deprecated

``` source
class CLKFullColorImageProvider
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

## Overview

All graphic complications support full-color images; however, some watch faces display these images as tinted images. Tinted images are black and white images with a highlight color that matches the watch face. If you don’t provide a tinted image provider, ClockKit automatically desaturates the full-color image to create the tinted image.

The template also often masks these image to produce circular images or rounded rectangles.

For information about the image sizes and masks, see Apple Watch Human Interface Guidelines.

## Topics

### Creating an Image Provider

convenience init(fullColorImage: UIImage)

Creates an image provider with the specified full-color image.

convenience init(fullColorImage: UIImage, tintedImageProvider: CLKImageProvider?)

Creates an image provider that produces full-color and tinted images.

### Getting the Image Data

var image: UIImage

The full-color image to display.

var tintedImageProvider: CLKImageProvider?

An image provider that produces alternative images for tinted graphic complications.

### Setting the Accessibility Label

var accessibilityLabel: String?

A succinct label that identifies the purpose of the image.

### Creating Empty Image Providers

init()

Creates an empty full color image provider.

class func new() -> Self

Creates an empty full color image provider.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Image providers

class CLKImageProvider

An image displayed by a complication.

Deprecated

