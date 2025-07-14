

- ImageCaptureCore
-  ICCameraItemMetadataOption 

Structure

# ICCameraItemMetadataOption

An option for the item’s metadata.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
struct ICCameraItemMetadataOption
```

## Topics

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Requesting Metadata

func requestMetadata()

Requests metadata for the item.

var metadata: [AnyHashable : Any]?

The item’s metadata.

var metadataIfAvailable: [String : Any]?

The item’s metadata if it is readily available.

func flushMetadataCache()

Deletes the item’s cached metadata.

