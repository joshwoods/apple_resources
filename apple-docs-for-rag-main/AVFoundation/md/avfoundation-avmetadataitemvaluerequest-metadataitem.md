

- AVFoundation
- AVMetadataItemValueRequest
-  metadataItem 

Instance Property

# metadataItem

The metadata item to request a value for.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
weak var metadataItem: AVMetadataItem? { get }
```

## See Also

### Handling the Response

func respond(value: any NSCopying &amp; NSObjectProtocol)

Returns the metadata item’s value.

func respond(error: any Error)

Returns an error when the system fails to load the value.

