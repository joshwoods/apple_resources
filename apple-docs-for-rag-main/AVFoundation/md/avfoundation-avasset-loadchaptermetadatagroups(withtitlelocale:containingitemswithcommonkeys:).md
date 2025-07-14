

- AVFoundation
- AVAsset
-  loadChapterMetadataGroups(withTitleLocale:containingItemsWithCommonKeys:) 

Instance Method

# loadChapterMetadataGroups(withTitleLocale:containingItemsWithCommonKeys:)

Loads chapter metadata that contains the specified title locale and common keys.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func loadChapterMetadataGroups(
    withTitleLocale locale: Locale,
    containingItemsWithCommonKeys commonKeys: [AVMetadataKey] = []
) async throws -> [AVTimedMetadataGroup]
```

## Parameters 

`locale`  

The locale of the chapter metadata to load.

`commonKeys`  

An array of common AVMetadataKey values to include in the returned array. The framework currently only supports the commonKeyArtwork key.

## Return Value

An array of chapter metadata items for a locale.

## Discussion

This method returns an array of AVTimedMetadataGroup objects asynchronously. Each object in the array contains an AVMetadataItem that represents the chapter’s title, and the metadata group’s timeRange value equals the time range of the chapter title item.

The metadata group contains all chapter metadata, including items with the common key commonKeyArtwork, if such items are present. The system adds an AVMetadataItem with the specified common key to an existing AVTimedMetadataGroup object if the time range (timestamp and duration) of the metadata item and the metadata group overlap. The locales of such items don’t need to match the locale of the chapter titles.

You can use the metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:) method to further filter the metadata items in each group. You can also filter the returned items based on locale using the metadataItems(from:with:) method.

## See Also

### Loading Chapter Metadata

static var availableChapterLocales: AVAsyncProperty&lt;Root, [Locale]>

The locales of an asset’s chapter metadata.

func loadChapterMetadataGroups(bestMatchingPreferredLanguages: [String], completionHandler: ([AVTimedMetadataGroup]?, (any Error)?) -> Void)

Loads chapter metadata with a locale that best matches the list of preferred languages.

