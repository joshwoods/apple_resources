

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  removeFirst() 

Instance Method

# removeFirst()

Removes and returns the first element of the collection.

MusicKitSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
@discardableResult
mutating func removeFirst() -> Self.Element
```

## Return Value

The removed element.

## Discussion

The collection must not be empty.

```
var bugs = ["Aphid", "Bumblebee", "Cicada", "Damselfly", "Earwig"]
bugs.removeFirst()
print(bugs)
// Prints "["Bumblebee", "Cicada", "Damselfly", "Earwig"]"
```

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

