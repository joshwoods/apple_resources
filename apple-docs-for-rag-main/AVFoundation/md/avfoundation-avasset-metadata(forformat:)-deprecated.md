

- AVFoundation
- AVAsset
-  metadata(forFormat:) Deprecated

Instance Method

# metadata(forFormat:)

Returns an array of metadata items from the container with the specified format.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func metadata(forFormat format: AVMetadataFormat) -> [AVMetadataItem]
```

Deprecated

Use loadMetadata(for:completionHandler:) instead.

## Parameters 

`format`  

The metadata format for which you want items.

## Return Value

An array of AVMetadataItem objects, one for each metadata item in the container of the specified format, or an empty array if there is no metadata for the specified format.

## Discussion

You can filter the array to the specific items of interest using the class methods provided by AVMetadataItem, like metadataItems(from:filteredByIdentifier:) or metadataItems(from:with:).

You can call this method without blocking the current thread after you’ve asynchronously loaded the availableMetadataFormats property.

