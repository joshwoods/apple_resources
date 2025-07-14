

- ImageCaptureCore
- ICCameraItem
-  largeThumbnailIfAvailable 

Instance Property

# largeThumbnailIfAvailable

A large thumbnail for the item if one is readily available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.15DeprecatedvisionOS 1.0+

``` source
var largeThumbnailIfAvailable: CGImage? { get }
```

## Discussion

If a large thumbnail is not readily available, accessing this property requests it from the device.

When the thumbnail is received, cameraDevice(_:didReceiveThumbnailFor:) is called on the the device’s delegate.

Execution of the delegate callback occurs on the main thread.

## See Also

### Requesting Thumbnails

func requestThumbnail()

Requests a thumbnail for the item.

var thumbnail: CGImage?

The item’s thumbnail.

var thumbnailIfAvailable: CGImage?

The item’s thumbnail if it is readily available.

func flushThumbnailCache()

Deletes the item’s cached thumbnail.

struct ICCameraItemThumbnailOption

An option for the item’s thumbnail.

