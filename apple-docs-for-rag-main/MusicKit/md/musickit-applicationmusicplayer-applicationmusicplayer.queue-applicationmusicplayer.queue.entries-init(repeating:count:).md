

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  init(repeating:count:) 

Initializer

# init(repeating:count:)

Creates a new collection containing the specified number of a single, repeated value.

MusicKitSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
init(
    repeating repeatedValue: Self.Element,
    count: Int
)
```

## Parameters 

`repeatedValue`  

The element to repeat.

`count`  

The number of times to repeat the value passed in the `repeating` parameter. `count` must be zero or greater.

## Discussion

Here’s an example of creating an array initialized with five strings containing the letter *Z*.

```
let fiveZs = Array(repeating: "Z", count: 5)
print(fiveZs)
// Prints "["Z", "Z", "Z", "Z", "Z"]"
```

