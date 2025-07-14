

- AVFoundation
- AVAsset
-  commonMetadata Deprecated

Instance Property

# commonMetadata

The metadata items an asset contains for common metadata identifiers that provide a value.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var commonMetadata: [AVMetadataItem] { get }
```

Deprecated

Load the value of commonMetadata asynchronously instead.

## Discussion

This property value is an array of metadata items, one for each metadata key from the common key space for which the asset has an available value. You can use the various class methods provided by AVMetadataItem, such as metadataItems(from:filteredByIdentifier:) or metadataItems(from:with:) to filter the array to the specific items of interest.

