

- AVFoundation
-  AVMutableCaptionRegion 

Class

# AVMutableCaptionRegion

A mutable caption region subclass that you use to create new caption regions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVMutableCaptionRegion
```

## Topics

### Creating a Caption Region

init()

Creates a caption region.

init(identifier: String)

Creates a caption region that has an identifier.

### Configuring the Region

var origin: AVCaptionPoint

The region’s top-left position.

var size: AVCaptionSize

The height and width of the region.

var displayAlignment: AVCaptionRegion.DisplayAlignment

The alignment of lines for the region.

var scroll: AVCaptionRegion.Scroll

The scroll mode of the region.

var writingMode: AVCaptionRegion.WritingMode

The block and inline progression direction of the region.

## Relationships

### Inherits From

- AVCaptionRegion

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Regions

class AVCaptionRegion

An object that represents the region in which the system presents a caption.

