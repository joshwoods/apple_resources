

- AVFoundation
- AVComposition
-  chapterMetadataGroups(withTitleLocale:containingItemsWithCommonKeys:) 

Instance Method

# chapterMetadataGroups(withTitleLocale:containingItemsWithCommonKeys:)

Returns an array of chapters that contain the specified title locale and common keys.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func chapterMetadataGroups(
    withTitleLocale locale: Locale,
    containingItemsWithCommonKeys commonKeys: [AVMetadataKey]?
) -> [AVTimedMetadataGroup]
```

## Parameters 

`locale`  

The locale of the metadata items carrying chapter titles.

`commonKeys`  

An array of common keys of AVMetadataItem to include in the returned array. The framework currently only supports the commonKeyArtwork key.

## Return Value

An array of AVTimedMetadataGroup objects.

## Discussion

A metadata group contains an AVMetadataItem object that represents the chapter title, and a time range equal to the time range of the chapter title item.

The system adds a metadata item with the specified common key to an existing AVTimedMetadataGroup object if the time range (timestamp and duration) of the metadata item and the metadata group overlap.

The locale of items that don’t contain chapter titles doesn’t need to match the specified locale parameter. You can filter the returned items based on locale using metadataItems(from:with:).

## See Also

### Accessing Chapter Metadata

var availableChapterLocales: [Locale]

The locales of the asset’s chapter metadata.

func chapterMetadataGroups(bestMatchingPreferredLanguages: [String]) -> [AVTimedMetadataGroup]

Returns an array of chapters with a locale that best matches the list of preferred languages.

