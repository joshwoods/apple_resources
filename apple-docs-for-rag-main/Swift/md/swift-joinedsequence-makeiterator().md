

- Swift
- JoinedSequence
-  makeIterator() 

Instance Method

# makeIterator()

Return an iterator over the elements of this sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func makeIterator() -> JoinedSequence.Iterator
```

Available when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

## Discussion

Complexity

O(1).

