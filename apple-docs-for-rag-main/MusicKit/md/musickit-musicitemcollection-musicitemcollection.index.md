

- MusicKit
- MusicItemCollection
-  MusicItemCollection.Index 

Type Alias

# MusicItemCollection.Index

A type that represents a position in the collection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias Index = Array.Index
```

Available when `MusicItemType` conforms to `MusicItem`.

## Discussion

Valid indices consist of the position of every element and a “past the end” position that’s not valid for use as a subscript argument.

