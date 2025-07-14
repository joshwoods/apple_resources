

- Swift
- AsyncSequence
-  AsyncIterator 

Associated Type

# AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
associatedtype AsyncIterator : AsyncIteratorProtocol
```

**Required**

## See Also

### Creating an Iterator

func makeAsyncIterator() -> Self.AsyncIterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

**Required**

protocol AsyncIteratorProtocol

A type that asynchronously supplies the values of a sequence one at a time.

associatedtype Element

The type of element produced by this asynchronous sequence.

**Required**

