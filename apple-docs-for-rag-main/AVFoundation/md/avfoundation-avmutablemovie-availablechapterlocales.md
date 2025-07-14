

- AVFoundation
- AVMutableMovie
-  availableChapterLocales 

Instance Property

# availableChapterLocales

The locales of the asset’s chapter metadata.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+watchOS 1.0+

``` source
var availableChapterLocales: [Locale] { get }
```

## See Also

### Accessing Chapter Metadata

func chapterMetadataGroups(bestMatchingPreferredLanguages: [String]) -> [AVTimedMetadataGroup]

Returns an array of chapters with a locale that best matches the list of preferred languages.

func chapterMetadataGroups(withTitleLocale: Locale, containingItemsWithCommonKeys: [AVMetadataKey]?) -> [AVTimedMetadataGroup]

Returns an array of chapters that contain the specified title locale and common keys.

