

- MusicKit
- MusicLibrarySectionedRequest
-  filterSections(matching:equalTo:) 

Instance Method

# filterSections(matching:equalTo:)

Filters sections by a given optional property that matches a specific value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func filterSections(
    matching keyPath: KeyPath,
    equalTo value: Value?
) where SectionType : MusicLibraryRequestable, Value : MusicLibraryRequestFilterValueEquatable
```

