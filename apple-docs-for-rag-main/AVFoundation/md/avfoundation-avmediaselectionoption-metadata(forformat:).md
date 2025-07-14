

- AVFoundation
- AVMediaSelectionOption
-  metadata(forFormat:) 

Instance Method

# metadata(forFormat:)

Returns an array of metadata items—one for each metadata item in the container of a given format.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func metadata(forFormat format: String) -> [AVMetadataItem]
```

## Parameters 

`format`  

The metadata format for which items are requested.

## Return Value

An array of `AVMetadataItem` objects, one for each metadata item in the container of format, or `nil` if there is no metadata of the specified format.

## See Also

### Managing Metadata

var commonMetadata: [AVMetadataItem]

An array of metadata items for each common metadata key for which a value is available.

var availableMetadataFormats: [String]

The metadata formats that contain metadata associated with the option.

