

- AVFoundation
- AVMetadataItem
-  metadataItems(from:filteredByIdentifier:) 

Type Method

# metadataItems(from:filteredByIdentifier:)

Returns metadata items for the specified identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func metadataItems(
    from metadataItems: [AVMetadataItem],
    filteredByIdentifier identifier: AVMetadataIdentifier
) -> [AVMetadataItem]
```

## Parameters 

`metadataItems`  

The metadata items to filter.

`identifier`  

The identifier of the metadata items to retrieve.

## Return Value

An array of metadata items that match the specified identifier.

## Mentioned in 

Retrieving media metadata

## See Also

### Filtering Arrays of Metadata Items

class func metadataItems(from: [AVMetadataItem], withKey: Any?, keySpace: AVMetadataKeySpace?) -> [AVMetadataItem]

Returns metadata items that match a specified key or key space.

class func metadataItems(from: [AVMetadataItem], with: Locale) -> [AVMetadataItem]

Returns metadata items that match a specified locale.

class func metadataItems(from: [AVMetadataItem], filteredAndSortedAccordingToPreferredLanguages: [String]) -> [AVMetadataItem]

Returns metadata items whose locales match one of the specified language identifiers.

class func metadataItems(from: [AVMetadataItem], filteredBy: AVMetadataItemFilter) -> [AVMetadataItem]

Returns filtered metadata items.

