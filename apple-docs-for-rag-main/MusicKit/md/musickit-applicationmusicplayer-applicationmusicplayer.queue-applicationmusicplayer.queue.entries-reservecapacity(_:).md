

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  reserveCapacity(\_:) 

Instance Method

# reserveCapacity(\_:)

Prepares the collection to store the specified number of elements, when doing so is appropriate for the underlying type.

MusicKitSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
mutating func reserveCapacity(_ n: Int)
```

## Parameters 

`n`  

The requested number of elements to store.

## Discussion

If you will be adding a known number of elements to a collection, use this method to avoid multiple reallocations. A type that conforms to `RangeReplaceableCollection` can choose how to respond when this method is called. Depending on the type, it may make sense to allocate more or less storage than requested or to take no action at all.

