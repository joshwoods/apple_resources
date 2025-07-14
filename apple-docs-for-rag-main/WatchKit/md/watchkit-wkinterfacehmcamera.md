

- WatchKit
-  WKInterfaceHMCamera 

Class

# WKInterfaceHMCamera

An interface element that displays either a video stream or a single snapshot from an IP camera connected to HomeKit.

watchOS 3.0+

``` source
class WKInterfaceHMCamera
```

## Overview

Do not subclass or create instances of this class yourself. Instead, define an outlet in your interface controller class and connect it to the corresponding object in your storyboard file. For example, to refer to a camera interface object in your interface, define a property with the following syntax in your interface controller class:

- Swift
- Objective-C

```
@IBOutlet weak var myCamera: WKInterfaceHMCamera!
```

```
@property (weak, nonatomic) IBOutlet WKInterfaceHMCamera* myCamera;
```

During the initialization of your interface controller, WatchKit creates the camera interface object and assigns it to its associated outlet. At that point, you can use the camera interface object to change to the onscreen content.

The camera interface object in your Watch app must be connected to a WKInterfaceHMCamera outlet in your WatchKit extension for the camera to be visible in your watchOS app’s user interface.

## Topics

### Setting the Camera Source

func setCameraSource(HMCameraSource?)

Set the HomeKit camera source displayed by this interface object.

### Initializing for SwiftUI

init()

Creates a camera for use in SwiftUI.

Deprecated

## Relationships

### Inherits From

- WKInterfaceObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Images and movies

class WKInterfaceImage

An image that can be displayed in the interface of your watchOS app.

class WKImage

A wrapper for images you use with a picker interface.

protocol WKImageAnimatable

A collection of methods you can use to control the playback of animated images.

class WKInterfaceMovie

An interface element that lets you play video and audio content in your watchOS app.

class WKInterfaceInlineMovie

An interface element that displays a video’s poster image and supports inline playing of the video.

enum WKVideoGravity

Constants indicating the appearance of video content.

