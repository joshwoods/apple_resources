

- Core Video
-  CVFillExtendedPixelsCallBackData 

Structure

# CVFillExtendedPixelsCallBackData

A structure for holding information that describes a custom extended pixel fill algorithm.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CVFillExtendedPixelsCallBackData
```

## Overview

You must fill out this structure and store it as part of your pixel format description Core Foundation dictionary (key: `kCVPixelFormatFillExtendedPixelsCallback`, type: `CFData`). However, if your custom pixel format never needs the functionality of CVPixelBufferFillExtendedPixels(_:), you don’t need to add this key or implement the associated callback.

For more information about defining a custom pixel format, see Pixel Format Description Keys.

## Topics

### Initializers

init()

init(version: CFIndex, fillCallBack: CVFillExtendedPixelsCallBack?, refCon: UnsafeMutableRawPointer?)

### Properties

var fillCallBack: CVFillExtendedPixelsCallBack?

var refCon: UnsafeMutableRawPointer?

A pointer to application-defined data that is passed to your custom pixel fill function.

var version: CFIndex

The version of this fill algorithm.

## Relationships

### Conforms To

- BitwiseCopyable

