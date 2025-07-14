

- MusicKit
- MusicPlayer
- MusicPlayer.Queue
- MusicPlayer.Queue.EntryInsertionPosition
-  MusicPlayer.Queue.EntryInsertionPosition.afterCurrentEntry 

Case

# MusicPlayer.Queue.EntryInsertionPosition.afterCurrentEntry

A position that allows prepending entries in the playback queue, similar to the Play Next feature in the Music app.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
case afterCurrentEntry
```

## Discussion

Inserting entries after the current one merely enqueues them to play next, and lets the current entry finish playing to the end.

Alternatively, you may change the current entry programmatically by setting the `currentEntry` property of the queue or queue.

