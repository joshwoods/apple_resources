

- ImageCaptureCore
- ICCameraItem
-  requestMetadata() 

Instance Method

# requestMetadata()

Requests metadata for the item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func requestMetadata()
```

## Discussion

If metadata for the item is not readily available, accessing this property requests metadata from the camera, then notifies the delegate by calling cameraDevice(_:didReceiveMetadata:for:error:).

Execution of the delegate callback occurs on the main thread.

## See Also

### Requesting Metadata

var metadata: [AnyHashable : Any]?

The item’s metadata.

var metadataIfAvailable: [String : Any]?

The item’s metadata if it is readily available.

func flushMetadataCache()

Deletes the item’s cached metadata.

struct ICCameraItemMetadataOption

An option for the item’s metadata.

