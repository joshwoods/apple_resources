

- MusicKit
- MusicItemCollection
-  drop(while:) 

Instance Method

# drop(while:)

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

MusicKitSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func drop(while predicate: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence
```

## Parameters 

`predicate`  

A closure that takes an element of the sequence as its argument and returns `true` if the element should be skipped or `false` if it should be included. Once the predicate returns `false` it will not be called again.

## Discussion

Complexity

O(*n*), where *n* is the length of the collection.

