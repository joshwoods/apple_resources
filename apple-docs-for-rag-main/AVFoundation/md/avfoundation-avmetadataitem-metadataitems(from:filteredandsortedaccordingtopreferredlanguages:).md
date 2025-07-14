

- AVFoundation
- AVMetadataItem
-  metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:) 

Type Method

# metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:)

Returns metadata items whose locales match one of the specified language identifiers.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func metadataItems(
    from metadataItems: [AVMetadataItem],
    filteredAndSortedAccordingToPreferredLanguages preferredLanguages: [String]
) -> [AVMetadataItem]
```

## Parameters 

`metadataItems`  

The metadata items to filter.

`preferredLanguages`  

An array of NSString objects, each of which contains a canonicalized IETF BCP 47 language identifier. The order of the identifiers in the array reflects the preferred language order, with the most preferred language being first in the array. Typically, you pass the user’s preferred languages by retrieving this array from the preferredLanguages class method of NSLocale.

## Return Value

An array of metadata items that match the specified languages.

## See Also

### Filtering Arrays of Metadata Items

class func metadataItems(from: [AVMetadataItem], filteredByIdentifier: AVMetadataIdentifier) -> [AVMetadataItem]

Returns metadata items for the specified identifier.

class func metadataItems(from: [AVMetadataItem], withKey: Any?, keySpace: AVMetadataKeySpace?) -> [AVMetadataItem]

Returns metadata items that match a specified key or key space.

class func metadataItems(from: [AVMetadataItem], with: Locale) -> [AVMetadataItem]

Returns metadata items that match a specified locale.

class func metadataItems(from: [AVMetadataItem], filteredBy: AVMetadataItemFilter) -> [AVMetadataItem]

Returns filtered metadata items.

