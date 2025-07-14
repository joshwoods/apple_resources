

- MusicKit
- MusicLibrarySectionedRequest
-  filterSections(matching:contains:) 

Instance Method

# filterSections(matching:contains:)

Filters sections by a given optional property that contains a specific string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func filterSections(
    matching keyPath: KeyPath,
    contains text: String
) where SectionType : MusicLibraryRequestable
```

