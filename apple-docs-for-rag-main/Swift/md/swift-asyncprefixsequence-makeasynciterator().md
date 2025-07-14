

- Swift
- AsyncPrefixSequence
-  makeAsyncIterator() 

Instance Method

# makeAsyncIterator()

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func makeAsyncIterator() -> AsyncPrefixSequence.Iterator
```

Available when `Base` conforms to `AsyncSequence`.

## Return Value

An instance of the `AsyncIterator` type used to produce elements of the asynchronous sequence.

