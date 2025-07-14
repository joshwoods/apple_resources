

- MusicKit
- ApplicationMusicPlayer
- ApplicationMusicPlayer.Queue
- ApplicationMusicPlayer.Queue.Entries
-  filter(\_:) 

Instance Method

# filter(\_:)

Returns a new collection of the same type containing, in order, the elements of the original collection that satisfy the given predicate.

MusicKitSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+Swift 4.0+

``` source
func filter(_ isIncluded: (Self.Element) throws -> Bool) rethrows -> Self
```

## Parameters 

`isIncluded`  

A closure that takes an element of the sequence as its argument and returns a Boolean value indicating whether the element should be included in the returned collection.

## Return Value

A collection of the elements that `isIncluded` allowed.

## Discussion

In this example, `filter(_:)` is used to include only names shorter than five characters.

```
let cast = ["Vivien", "Marlon", "Kim", "Karl"]
let shortNames = cast.filter { $0.count 

Complexity

O(*n*), where *n* is the length of the collection.

