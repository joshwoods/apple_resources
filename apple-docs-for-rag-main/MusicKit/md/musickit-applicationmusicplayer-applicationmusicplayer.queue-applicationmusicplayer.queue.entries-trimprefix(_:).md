

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  trimPrefix(\_:) 

Instance Method

# trimPrefix(\_:)

Removes `prefix` from the start of the collection.

MusicKitSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func trimPrefix(_ prefix: Prefix) where Prefix : Sequence, Self.Element == Prefix.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`prefix`  

The collection to remove from this collection.

