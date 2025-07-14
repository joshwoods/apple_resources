

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  removeFirst(\_:) 

Instance Method

# removeFirst(\_:)

Removes the specified number of elements from the beginning of the collection.

MusicKitSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
mutating func removeFirst(_ k: Int)
```

## Parameters 

`k`  

The number of elements to remove from the collection. `k` must be greater than or equal to zero and must not exceed the number of elements in the collection.

## Discussion

```
var bugs = ["Aphid", "Bumblebee", "Cicada", "Damselfly", "Earwig"]
bugs.removeFirst(3)
print(bugs)
// Prints "["Damselfly", "Earwig"]"
```

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

