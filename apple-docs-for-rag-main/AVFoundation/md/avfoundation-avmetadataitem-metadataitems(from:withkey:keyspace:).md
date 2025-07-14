

- AVFoundation
- AVMetadataItem
-  metadataItems(from:withKey:keySpace:) 

Type Method

# metadataItems(from:withKey:keySpace:)

Returns metadata items that match a specified key or key space.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func metadataItems(
    from metadataItems: [AVMetadataItem],
    withKey key: Any?,
    keySpace: AVMetadataKeySpace?
) -> [AVMetadataItem]
```

## Parameters 

`metadataItems`  

The metadata items to filter.

`key`  

The key of the metadata items to retrieve, or `nil` if you don’t want to filter by key.

`keySpace`  

The key space of the metadata items to retrieve, or `nil` if you don’t want to filter by key space.

## Return Value

An array of metadata items that match the specified key and key space.

## See Also

### Filtering Arrays of Metadata Items

class func metadataItems(from: [AVMetadataItem], filteredByIdentifier: AVMetadataIdentifier) -> [AVMetadataItem]

Returns metadata items for the specified identifier.

class func metadataItems(from: [AVMetadataItem], with: Locale) -> [AVMetadataItem]

Returns metadata items that match a specified locale.

class func metadataItems(from: [AVMetadataItem], filteredAndSortedAccordingToPreferredLanguages: [String]) -> [AVMetadataItem]

Returns metadata items whose locales match one of the specified language identifiers.

class func metadataItems(from: [AVMetadataItem], filteredBy: AVMetadataItemFilter) -> [AVMetadataItem]

Returns filtered metadata items.

