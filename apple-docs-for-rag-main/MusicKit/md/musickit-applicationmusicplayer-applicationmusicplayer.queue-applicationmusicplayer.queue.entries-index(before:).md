

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  index(before:) 

Instance Method

# index(before:)

Returns the position immediately before the given index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
func index(before i: ApplicationMusicPlayer.Queue.Entries.Index) -> ApplicationMusicPlayer.Queue.Entries.Index
```

## Parameters 

`i`  

A valid index of the collection. `i` must be greater than `startIndex`.

## Return Value

The index value immediately before `i`.

