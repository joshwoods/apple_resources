

- AVFoundation
- AVAsset
-  chapterMetadataGroups(bestMatchingPreferredLanguages:) Deprecated

Instance Method

# chapterMetadataGroups(bestMatchingPreferredLanguages:)

Returns an array of chapters with a locale that best matches the list of preferred languages.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func chapterMetadataGroups(bestMatchingPreferredLanguages preferredLanguages: [String]) -> [AVTimedMetadataGroup]
```

Deprecated

Use loadChapterMetadataGroups(bestMatchingPreferredLanguages:completionHandler:) instead.

## Parameters 

`preferredLanguages`  

An array of BCP 47 language identifier strings. The order of the identifiers in the array reflects the preferred language order, with the most preferred language being first in the array. Typically, you pass the user’s preferred languages by retrieving this array from the preferredLanguages class method of NSLocale.

## Return Value

An array of AVTimedMetadataGroup objects.

## Mentioned in 

Presenting Chapter Markers

## Discussion

Each object in the returned array contains an AVMetadataItem object representing the chapter title. The time range property of the AVTimedMetadataGroup object is equal to the time range of the chapter title item.

The metadata group contains all chapter metadata, including items with the common key commonKeyArtwork, if such items are present. The system adds an AVMetadataItem with the specified common key to an existing AVTimedMetadataGroup object if the time range (timestamp and duration) of the metadata item and the metadata group overlap. The locale of such items don’t need to match the locale of the chapter titles.

You can use the metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:) method to further filter the metadata items in each group. You can also filter the returned items based on locale using the metadataItems(from:with:) method.

This method is callable without blocking the current thread after you’ve asynchronously loaded the availableChapterLocales property.

