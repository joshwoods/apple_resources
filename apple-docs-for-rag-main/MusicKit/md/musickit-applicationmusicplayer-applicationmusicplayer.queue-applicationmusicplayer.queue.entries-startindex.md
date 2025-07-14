

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  startIndex 

Instance Property

# startIndex

The position of the first element in a nonempty collection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
var startIndex: ApplicationMusicPlayer.Queue.Entries.Index { get }
```

## Discussion

If the collection is empty, `startIndex` is equal to `endIndex`.

