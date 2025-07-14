

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  indices 

Instance Property

# indices

The indices that are valid for subscripting the collection, in ascending order.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
var indices: ApplicationMusicPlayer.Queue.Entries.Indices { get }
```

## Discussion

A collection’s `indices` property can hold a strong reference to the collection itself, causing the collection to be nonuniquely referenced. If you mutate the collection while iterating over its indices, a strong reference can result in an unexpected copy of the collection. To avoid the unexpected copy, use the `index(after:)` method starting with `startIndex` to produce indices instead.

```
var c = MyFancyCollection([10, 20, 30, 40, 50])
var i = c.startIndex
while i != c.endIndex {
    c[i] /= 5
    i = c.index(after: i)
}
// c == MyFancyCollection([2, 4, 6, 8, 10])
```

