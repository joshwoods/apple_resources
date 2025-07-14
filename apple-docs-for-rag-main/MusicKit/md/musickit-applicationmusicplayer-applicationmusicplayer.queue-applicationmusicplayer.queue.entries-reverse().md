

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  reverse() 

Instance Method

# reverse()

Reverses the elements of the collection in place.

MusicKitSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
mutating func reverse()
```

Available when `Self` conforms to `BidirectionalCollection`.

## Discussion

The following example reverses the elements of an array of characters:

```
var characters: [Character] = ["C", "a", "f", "é"]
characters.reverse()
print(characters)
// Prints "["é", "f", "a", "C"]"
```

Complexity

O(*n*), where *n* is the number of elements in the collection.

