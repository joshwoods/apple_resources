

- AVFoundation
- AVAssetTrack
-  metadata Deprecated

Instance Property

# metadata

An array of metadata items for all metadata identifiers that have a value.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.10–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var metadata: [AVMetadataItem] { get }
```

Deprecated

Load the value of metadata asynchronously instead.

## Discussion

You can filter the array of metadata items according to language using the metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:) method. Filter the results by identifier using the metadataItems(from:filteredByIdentifier:) method.

