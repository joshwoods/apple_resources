

- AVFoundation
- AVMediaSelectionOption
-  availableMetadataFormats 

Instance Property

# availableMetadataFormats

The metadata formats that contain metadata associated with the option.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var availableMetadataFormats: [String] { get }
```

## Discussion

The array contains `NSString` objects, each representing a metadata format that contains metadata associated with the option (for example, ID3, iTunes metadata, and so on).

## See Also

### Managing Metadata

var commonMetadata: [AVMetadataItem]

An array of metadata items for each common metadata key for which a value is available.

func metadata(forFormat: String) -> [AVMetadataItem]

Returns an array of metadata items—one for each metadata item in the container of a given format.

