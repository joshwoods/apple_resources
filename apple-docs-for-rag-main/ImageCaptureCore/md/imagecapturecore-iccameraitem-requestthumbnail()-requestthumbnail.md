

- ImageCaptureCore
- ICCameraItem
-  requestThumbnail() 

Instance Method

# requestThumbnail()

Requests a thumbnail for the item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func requestThumbnail()
```

## Discussion

If a thumbnail is not readily available, accessing this property will send a message to the device requesting a thumbnail for the file. The delegate of the device will be notified via method cameraDevice(_:didReceiveThumbnail:for:error:), if this method is implemented by the delegate. Execution of the delegate callback will occur on the main thread.

## See Also

### Requesting Thumbnails

var thumbnail: CGImage?

The item’s thumbnail.

var thumbnailIfAvailable: CGImage?

The item’s thumbnail if it is readily available.

var largeThumbnailIfAvailable: CGImage?

A large thumbnail for the item if one is readily available.

func flushThumbnailCache()

Deletes the item’s cached thumbnail.

struct ICCameraItemThumbnailOption

An option for the item’s thumbnail.

