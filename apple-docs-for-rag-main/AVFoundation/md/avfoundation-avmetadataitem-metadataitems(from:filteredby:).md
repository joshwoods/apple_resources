

- AVFoundation
- AVMetadataItem
-  metadataItems(from:filteredBy:) 

Type Method

# metadataItems(from:filteredBy:)

Returns filtered metadata items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func metadataItems(
    from metadataItems: [AVMetadataItem],
    filteredBy metadataItemFilter: AVMetadataItemFilter
) -> [AVMetadataItem]
```

## Parameters 

`metadataItems`  

The metadata items to filter.

`metadataItemFilter`  

The metadata item filter to apply.

## Return Value

The filtered array of metadata items.

## See Also

### Filtering Arrays of Metadata Items

class func metadataItems(from: [AVMetadataItem], filteredByIdentifier: AVMetadataIdentifier) -> [AVMetadataItem]

Returns metadata items for the specified identifier.

class func metadataItems(from: [AVMetadataItem], withKey: Any?, keySpace: AVMetadataKeySpace?) -> [AVMetadataItem]

Returns metadata items that match a specified key or key space.

class func metadataItems(from: [AVMetadataItem], with: Locale) -> [AVMetadataItem]

Returns metadata items that match a specified locale.

class func metadataItems(from: [AVMetadataItem], filteredAndSortedAccordingToPreferredLanguages: [String]) -> [AVMetadataItem]

Returns metadata items whose locales match one of the specified language identifiers.

