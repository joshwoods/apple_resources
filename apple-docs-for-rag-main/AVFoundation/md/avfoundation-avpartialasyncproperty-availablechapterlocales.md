

- AVFoundation
- AVPartialAsyncProperty
-  availableChapterLocales 

Type Property

# availableChapterLocales

The locales of an asset’s chapter metadata.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var availableChapterLocales: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Chapter Metadata

func loadChapterMetadataGroups(withTitleLocale: Locale, containingItemsWithCommonKeys: [AVMetadataKey]) async throws -> [AVTimedMetadataGroup]

Loads chapter metadata that contains the specified title locale and common keys.

func loadChapterMetadataGroups(bestMatchingPreferredLanguages: [String], completionHandler: ([AVTimedMetadataGroup]?, (any Error)?) -> Void)

Loads chapter metadata with a locale that best matches the list of preferred languages.

