

- WatchKit
-  WKImage 

Class

# WKImage

A wrapper for images you use with a picker interface.

watchOS 2.0+

``` source
class WKImage
```

## Overview

To create instances of this class, use one of the defined creation methods. Choose the method that best suits the image data you have. After creating the object, you can use associate it with a WKPickerItem object and use it in your picker interface.

## Topics

### Creating Image Objects

convenience init(image: UIImage)

Creates and returns an image object using the specified UIKit image.

convenience init(imageData: Data)

Creates an image with the specified raw image data.

convenience init(imageName: String)

Creates an image by loading an image file from the Watch app bundle.

### Getting the Image Data

var image: UIImage?

The UIKit image object

var imageData: Data?

The data object containing the raw image data.

var imageName: String?

The name of the image to load from the Watch app’s bundle.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Images and movies

class WKInterfaceImage

An image that can be displayed in the interface of your watchOS app.

protocol WKImageAnimatable

A collection of methods you can use to control the playback of animated images.

class WKInterfaceMovie

An interface element that lets you play video and audio content in your watchOS app.

class WKInterfaceInlineMovie

An interface element that displays a video’s poster image and supports inline playing of the video.

class WKInterfaceHMCamera

An interface element that displays either a video stream or a single snapshot from an IP camera connected to HomeKit.

enum WKVideoGravity

Constants indicating the appearance of video content.

