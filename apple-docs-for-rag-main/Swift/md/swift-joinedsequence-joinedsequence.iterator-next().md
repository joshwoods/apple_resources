

- Swift
- JoinedSequence
- JoinedSequence.Iterator
-  next() 

Instance Method

# next()

Advances to the next element and returns it, or `nil` if no next element exists.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func next() -> JoinedSequence.Iterator.Element?
```

Available when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

## Discussion

Once `nil` has been returned, all subsequent calls return `nil`.

