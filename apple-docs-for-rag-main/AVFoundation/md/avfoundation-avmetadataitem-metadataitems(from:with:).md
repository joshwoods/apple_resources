

- AVFoundation
- AVMetadataItem
-  metadataItems(from:with:) 

Type Method

# metadataItems(from:with:)

Returns metadata items that match a specified locale.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func metadataItems(
    from metadataItems: [AVMetadataItem],
    with locale: Locale
) -> [AVMetadataItem]
```

## Parameters 

`metadataItems`  

The metadata items to filter.

`locale`  

The locale of the metadata items to retrieve.

## Return Value

An array of metadata items that match the specified key and key space.

## See Also

### Filtering Arrays of Metadata Items

class func metadataItems(from: [AVMetadataItem], filteredByIdentifier: AVMetadataIdentifier) -> [AVMetadataItem]

Returns metadata items for the specified identifier.

class func metadataItems(from: [AVMetadataItem], withKey: Any?, keySpace: AVMetadataKeySpace?) -> [AVMetadataItem]

Returns metadata items that match a specified key or key space.

class func metadataItems(from: [AVMetadataItem], filteredAndSortedAccordingToPreferredLanguages: [String]) -> [AVMetadataItem]

Returns metadata items whose locales match one of the specified language identifiers.

class func metadataItems(from: [AVMetadataItem], filteredBy: AVMetadataItemFilter) -> [AVMetadataItem]

Returns filtered metadata items.

