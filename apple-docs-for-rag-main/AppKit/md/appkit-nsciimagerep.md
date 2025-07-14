

- AppKit
-  NSCIImageRep 

Class

# NSCIImageRep

An object that can render an image from a Core Image object.

macOS

``` source
class NSCIImageRep
```

## Topics

### Creating Representations of Core Image Objects

init(ciImage: CIImage)

Returns a representation of an image initialized to the specified Core Image instance.

### Getting Data

var ciImage: CIImage

The Core Image instance.

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

class NSPICTImageRep

An object that renders an image from a PICT format data stream of version 1, version 2, and extended version 2.

