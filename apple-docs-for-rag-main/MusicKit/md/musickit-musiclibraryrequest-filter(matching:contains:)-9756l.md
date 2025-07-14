

- MusicKit
- MusicLibraryRequest
-  filter(matching:contains:) 

Instance Method

# filter(matching:contains:)

Filters items by a given relationship that matches a specific value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func filter(
    matching keyPath: KeyPath?>,
    contains relatedItem: RelatedMusicItemType
) where RelatedMusicItemType : MusicItem
```

