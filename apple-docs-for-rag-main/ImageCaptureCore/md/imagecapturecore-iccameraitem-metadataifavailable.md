

- ImageCaptureCore
- ICCameraItem
-  metadataIfAvailable 

Instance Property

# metadataIfAvailable

The item’s metadata if it is readily available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.15DeprecatedvisionOS 1.0+

``` source
var metadataIfAvailable: [String : Any]? { get }
```

## Discussion

If metadata is not readily available, accessing this property will send a message to the device requesting metadata for the file. The delegate of the device will be notified via method cameraDevice(_:didReceiveMetadataFor:), if this method is implemented by the delegate. Execution of the delegate callback will occur on the main thread.

## See Also

### Requesting Metadata

func requestMetadata()

Requests metadata for the item.

var metadata: [AnyHashable : Any]?

The item’s metadata.

func flushMetadataCache()

Deletes the item’s cached metadata.

struct ICCameraItemMetadataOption

An option for the item’s metadata.

