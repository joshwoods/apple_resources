

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  index(after:) 

Instance Method

# index(after:)

Returns the position immediately after the given index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
func index(after i: ApplicationMusicPlayer.Queue.Entries.Index) -> ApplicationMusicPlayer.Queue.Entries.Index
```

## Parameters 

`i`  

A valid index of the collection. `i` must be less than `endIndex`.

## Return Value

The index value immediately after `i`.

## Discussion

The successor of an index must be well defined. For an index `i` into a collection `c`, calling `c.index(after: i)` returns the same index every time.

