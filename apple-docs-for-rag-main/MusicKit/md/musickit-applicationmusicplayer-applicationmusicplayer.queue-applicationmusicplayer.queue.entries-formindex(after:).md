

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  formIndex(after:) 

Instance Method

# formIndex(after:)

Replaces the given index with its successor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
func formIndex(after i: inout ApplicationMusicPlayer.Queue.Entries.Index)
```

## Parameters 

`i`  

A valid index of the collection. `i` must be less than `endIndex`.

