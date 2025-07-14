

- MusicKit
- MusicLibrarySection
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func == (a: MusicLibrarySection, b: MusicLibrarySection) -> Bool
```

Available when `SectionType` conforms to `MusicLibrarySectionRequestable`, `SectionType` conforms to `Equatable`, `MusicItemType` conforms to `MusicLibraryRequestable`, and `MusicItemType` conforms to `Equatable`.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

