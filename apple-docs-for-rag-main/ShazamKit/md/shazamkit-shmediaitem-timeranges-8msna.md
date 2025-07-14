

- ShazamKit
- SHMediaItem
-  timeRanges 

Instance Property

# timeRanges

An array of ranges that indicate the offsets within the reference signature that this media item describes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var timeRanges: [Range] { get }
```

## See Also

### Working with media item properties

subscript(SHMediaItemProperty) -> Any

Accesses the property for the specified key for reading.

struct SHMediaItemProperty

Constants for the media item property names.

var frequencySkewRanges: [Range&lt;Float>]

An array of ranges that indicate the frequency skews in the reference signature that this media item describes.

