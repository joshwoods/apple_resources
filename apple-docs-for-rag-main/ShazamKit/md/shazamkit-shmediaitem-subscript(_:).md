

- ShazamKit
- SHMediaItem
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the property for the specified key for reading.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(key: SHMediaItemProperty) -> Any { get }
```

## Parameters 

`key`  

The key for the media item property.

## Return Value

The value of the property; otherwise, `nil`.

## See Also

### Working with media item properties

struct SHMediaItemProperty

Constants for the media item property names.

var timeRanges: [Range&lt;TimeInterval>]

An array of ranges that indicate the offsets within the reference signature that this media item describes.

var frequencySkewRanges: [Range&lt;Float>]

An array of ranges that indicate the frequency skews in the reference signature that this media item describes.

