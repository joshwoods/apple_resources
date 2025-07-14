

- AVFoundation
- AVAsset
-  loadChapterMetadataGroups(bestMatchingPreferredLanguages:completionHandler:) 

Instance Method

# loadChapterMetadataGroups(bestMatchingPreferredLanguages:completionHandler:)

Loads chapter metadata with a locale that best matches the list of preferred languages.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func loadChapterMetadataGroups(
    bestMatchingPreferredLanguages preferredLanguages: [String],
    completionHandler: @escaping ([AVTimedMetadataGroup]?, (any Error)?) -> Void
)
```

``` source
func loadChapterMetadataGroups(bestMatchingPreferredLanguages preferredLanguages: [String]) async throws -> [AVTimedMetadataGroup]
```

## Parameters 

`preferredLanguages`  

An array of language identifiers in order of preference, each of which is an IETF BCP 47 (RFC 4646) language identifier. Call preferredLanguages to retrieve the list of languates the user prefers.

`completionHandler`  

A callback that the system invokes after it finishes the loading request. It passes the completion handler the following parameters:

metadataGroups  
An array of metadata groups, which may be empty if no groups exist for the specified languages. The value is `nil` if an error occurs.

error  
An error object if the request fails; otherwise, `nil`.

## Discussion

This method returns an array of AVTimedMetadataGroup objects asynchronously. Each object in the array contains an AVMetadataItem that represents the chapter’s title, and the metadata group’s timeRange value equals the time range of the chapter title item.

The metadata group contains all chapter metadata, including items with the common key commonKeyArtwork, if such items are present. The system adds an AVMetadataItem with the specified common key to an existing AVTimedMetadataGroup object if the time range (timestamp and duration) of the metadata item and the metadata group overlap. The locales of such items don’t need to match the locale of the chapter titles.

You can use the metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:) method to further filter the metadata items in each group. You can also filter the returned items based on locale using the metadataItems(from:with:) method.

## See Also

### Loading Chapter Metadata

static var availableChapterLocales: AVAsyncProperty&lt;Root, [Locale]>

The locales of an asset’s chapter metadata.

func loadChapterMetadataGroups(withTitleLocale: Locale, containingItemsWithCommonKeys: [AVMetadataKey]) async throws -> [AVTimedMetadataGroup]

Loads chapter metadata that contains the specified title locale and common keys.

