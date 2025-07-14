

- AppKit
-  NSPICTImageRep 

Class

# NSPICTImageRep

An object that renders an image from a PICT format data stream of version 1, version 2, and extended version 2.

macOS

``` source
class NSPICTImageRep
```

## Overview

Warning

There is no guarantee that the image will render exactly the same as it would under QuickDraw because of the differences between the display medium and QuickDraw. In particular, some transfer modes and region operations may not be supported.

## Topics

### Creating Representations of Images from PICT Data

init?(data: Data)

Returns a representation of an image from the specified data in the PICT file format.

### Getting Data

var boundingBox: NSRect

The rectangle that bounds the image representation.

var pictRepresentation: Data

The image representation’s PICT data.

## Relationships

### Inherits From

- NSImageRep

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Bitmap Formats

class NSBitmapImageRep

An object that renders an image from bitmap data.

class NSCIImageRep

An object that can render an image from a Core Image object.

