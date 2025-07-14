

- ImageCaptureCore
- ICCameraItem
-  thumbnail 

Instance Property

# thumbnail

The item’s thumbnail.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var thumbnail: CGImage? { get }
```

## Discussion

The value of this property is `nil` until you call requestThumbnail().

## See Also

### Requesting Thumbnails

func requestThumbnail()

Requests a thumbnail for the item.

var thumbnailIfAvailable: CGImage?

The item’s thumbnail if it is readily available.

var largeThumbnailIfAvailable: CGImage?

A large thumbnail for the item if one is readily available.

func flushThumbnailCache()

Deletes the item’s cached thumbnail.

struct ICCameraItemThumbnailOption

An option for the item’s thumbnail.

