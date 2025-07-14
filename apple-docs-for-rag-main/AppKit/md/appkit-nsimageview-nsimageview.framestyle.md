

- AppKit
- NSImageView
-  NSImageView.FrameStyle 

Enumeration

# NSImageView.FrameStyle

Constants that allow you to specify the kind of frame bordering the image.

macOS

``` source
enum FrameStyle
```

## Overview

These constants are used by imageFrameStyle. Note that some of these constants are stylistically obsolete and should be considered deprecated.

## Topics

### Constants

case none

An invisible frame

case photo

A thin black outline and a dropped shadow.

Deprecated

case grayBezel

A gray, concave bezel that makes the image look sunken.

case groove

A thin groove that looks etched around the image.

Deprecated

case button

A convex bezel that makes the image stand out in relief, like a button.

Deprecated

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum NSImageAlignment

Constants used by imageAlignment that allow you to specify the location of the image in the frame.

