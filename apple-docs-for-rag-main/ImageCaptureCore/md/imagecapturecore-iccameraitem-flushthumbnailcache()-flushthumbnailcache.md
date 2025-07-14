

- ImageCaptureCore
- ICCameraItem
-  flushThumbnailCache() 

Instance Method

# flushThumbnailCache()

Deletes the item’s cached thumbnail.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func flushThumbnailCache()
```

## See Also

### Requesting Thumbnails

func requestThumbnail()

Requests a thumbnail for the item.

var thumbnail: CGImage?

The item’s thumbnail.

var thumbnailIfAvailable: CGImage?

The item’s thumbnail if it is readily available.

var largeThumbnailIfAvailable: CGImage?

A large thumbnail for the item if one is readily available.

struct ICCameraItemThumbnailOption

An option for the item’s thumbnail.

