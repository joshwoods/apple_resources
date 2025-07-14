

- MusicKit
-  MusicLibrarySection 

Structure

# MusicLibrarySection

A section for a library sectioned response.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@dynamicMemberLookup
struct MusicLibrarySection where SectionType : MusicLibrarySectionRequestable, MusicItemType : MusicLibraryRequestable
```

## Overview

Your app can access any property of the requested section type directly on this library section object.

Your app can also access the items contained in a library section with the items property.

## Topics

### Instance Properties

let items: MusicItemCollection&lt;MusicItemType>

A collection of items that correspond to the children of the section.

### Subscripts

subscript&lt;T>(dynamicMember _: KeyPath&lt;SectionType, T>) -> T

A subscript that allows your app to access any property of the requested section type directly on this library section object.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- Sendable

