

- AVFoundation
- AVAssetTrack
-  metadata(forFormat:) Deprecated

Instance Method

# metadata(forFormat:)

Returns metadata items that a track contains for the specified format.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func metadata(forFormat format: AVMetadataFormat) -> [AVMetadataItem]
```

Deprecated

Use loadMetadata(for:completionHandler:) instead.

## Parameters 

`format`  

The format of the metadata items to retrieve.

## Return Value

An array of metadata items matching the specified format, or an empty array if none are found.

## Discussion

Apple discourages the use of this method in iOS 15, tvOS 15, and macOS 12 or later. Load track metadata asynchronously using loadMetadata(for:completionHandler:) instead.

You can call this method without blocking the current thread after you’ve loaded the availableMetadataFormats property.

