

- MusicKit
- MusicItemCollection
-  startIndex 

Instance Property

# startIndex

The position of the first element in a nonempty collection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var startIndex: MusicItemCollection.Index { get }
```

Available when `MusicItemType` conforms to `MusicItem`.

## Discussion

If the collection is empty, `startIndex` is equal to `endIndex`.

