

- MusicKit
-  MusicLibrarySectionedResponse 

Structure

# MusicLibrarySectionedResponse

An object that contains results for a library sectioned request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicLibrarySectionedResponse where SectionType : MusicLibrarySectionRequestable, MusicItemType : MusicLibraryRequestable
```

## Topics

### Instance Properties

let sections: [MusicLibrarySection&lt;SectionType, MusicItemType>]

An array of sections that match the filters on the originating library request.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

