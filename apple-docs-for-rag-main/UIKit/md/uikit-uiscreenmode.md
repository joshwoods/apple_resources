

- UIKit
-  UIScreenMode 

Class

# UIScreenMode

A possible set of attributes that can apply to a screen object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOS

``` source
class UIScreenMode
```

## Mentioned in 

Presenting content on a connected display

## Overview

A screen mode object encapsulates information about the size of the screen’s underlying display buffer and the aspect ratio it uses for individual pixels. Most developers should never need to use the information provided by this class and should simply use the bounds provided by the UIScreen object for their drawing space. The bounds of screen and window objects automatically take the pixel aspect ratio and underlying drawing hardware into consideration. However, developers that work with pixel-level information more directly may use the information in the current screen mode object to tailor their code for the target screen.

You don’t create instances of this class directly. Instead, you get the screen modes supported by a given screen from the corresponding UIScreen object.

## Topics

### Accessing the screen mode attributes

var size: CGSize

The screen size, measured in pixels.

var pixelAspectRatio: CGFloat

The aspect ratio of a single pixel.

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

### Screens

Presenting content on a connected display

Fill connected displays with additional content from your app.

class UIScreen

An object that defines the properties associated with a hardware-based display.

