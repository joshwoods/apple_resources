

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  formIndex(before:) 

Instance Method

# formIndex(before:)

Replaces the given index with its predecessor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
func formIndex(before i: inout ApplicationMusicPlayer.Queue.Entries.Index)
```

## Parameters 

`i`  

A valid index of the collection. `i` must be greater than `startIndex`.

