

- AVFoundation
- Media playback
-  Presenting Chapter Markers 

Article

# Presenting Chapter Markers

Add chapter markers to enable users to quickly navigate your content.

## Overview

Chapter markers enable users to quickly navigate your content. AVPlayerViewController automatically presents a chapter-selection interface if it finds chapter markers in the currently played asset. You can also directly retrieve this data whenever you want to create your own custom chapter-selection interface.

### Retrieve the Timed Metadata

Chapter markers are a type of timed metadata that apply only to ranges of time within the asset’s timeline. You retrieve an asset’s chapter metadata using either the chapterMetadataGroups(bestMatchingPreferredLanguages:) or chapterMetadataGroups(withTitleLocale:containingItemsWithCommonKeys:) methods. These methods become callable without blocking after you asynchronously load the value of the asset’s availableChapterLocales key.

```
let asset = AVAsset(url: )
let chapterLocalesKey = "availableChapterLocales"

asset.loadValuesAsynchronously(forKeys: [chapterLocalesKey]) {
    var error: NSError?
    let status = asset.statusOfValue(forKey: chapterLocalesKey, error: &error)
    if status == .loaded {
        let languages = Locale.preferredLanguages
        let chapterMetadata = asset.chapterMetadataGroups(bestMatchingPreferredLanguages: languages)
        // Process chapter metadata.
    }
    else {
        // Handle other status cases.
    }
}
```

### Convert Timed Metadata into Chapter Data

The value returned from the methods described above is an array of AVTimedMetadataGroup objects, each representing an individual chapter marker. An AVTimedMetadataGroup object contains a CMTimeRange, defining the time range to which its metadata applies, an array of AVMetadataItem objects representing the chapter’s title, and optionally, its thumbnail image. The following example shows how to convert the AVTimedMetadataGroup data into an array of custom model objects, called `Chapter`, to pass to the app’s view layer.

```
func convertTimedMetadataGroupsToChapters(groups: [AVTimedMetadataGroup]) -> [Chapter] {
    return groups.map { group in
        // Retrieve the title metadata items.
        let titleItems = AVMetadataItem.metadataItems(from: group.items,
                                                      filteredByIdentifier: .commonIdentifierTitle)

        // Retrieve the artwork metadata items.
        let artworkItems = AVMetadataItem.metadataItems(from: group.items,
                                                        filteredByIdentifier: .commonIdentifierArtwork)

        var title = "Default Title"
        var image = UIImage(named: "placeholder")!

        if let titleValue = titleItems.first?.stringValue {
            title = titleValue
        }

        if let imgData = artworkItems.first?.dataValue, let imageValue = UIImage(data: imgData) {
            image = imageValue
        }

        return Chapter(time: group.timeRange.start, title: title, image: image)
    }
}
```

With the relevant data converted, you can build a chapter-selection interface and use the time value of the chapter object to seek the current presentation using an AVPlayer object’s seek(to:) method.

## See Also

### Timed metadata

class AVMetadataGroup

A collection of metadata items associated with a timeline segment.

class AVTimedMetadataGroup

A collection of metadata items that are valid for use during a specific time range.

class AVMutableTimedMetadataGroup

A mutable collection of metadata items that are valid for use during a specific time range.

class AVDateRangeMetadataGroup

A collection of metadata items that are valid for use within a specific date range.

class AVMutableDateRangeMetadataGroup

A mutable collection of metadata items that are valid for use within a specific range of dates.

class AVPlayerItemMediaDataCollector

The abstract base for media data collectors.

class AVPlayerItemMetadataCollector

An object used to capture the date range metadata defined for an HTTP Live Streaming asset.

