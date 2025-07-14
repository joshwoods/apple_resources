

- AVFoundation
-  AVMetadataItemValueRequest 

Class

# AVMetadataItemValueRequest

An object that responds to a request to load the value of a metadata item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVMetadataItemValueRequest
```

## Topics

### Handling the Response

func respond(value: any NSCopying &amp; NSObjectProtocol)

Returns the metadata item’s value.

func respond(error: any Error)

Returns an error when the system fails to load the value.

var metadataItem: AVMetadataItem?

The metadata item to request a value for.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating a Metadata Item

init(propertiesOfMetadataItem: AVMetadataItem, valueLoadingHandler: (AVMetadataItemValueRequest) -> Void)

Creates a metadata item whose value loads on an on-demand basis only.

