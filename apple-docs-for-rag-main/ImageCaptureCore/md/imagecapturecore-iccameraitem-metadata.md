

- ImageCaptureCore
- ICCameraItem
-  metadata 

Instance Property

# metadata

The item’s metadata.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var metadata: [AnyHashable : Any]? { get }
```

## Discussion

The value of this property is `nil` unless a requestMetadata() message is sent to this object.

## See Also

### Requesting Metadata

func requestMetadata()

Requests metadata for the item.

var metadataIfAvailable: [String : Any]?

The item’s metadata if it is readily available.

func flushMetadataCache()

Deletes the item’s cached metadata.

struct ICCameraItemMetadataOption

An option for the item’s metadata.

