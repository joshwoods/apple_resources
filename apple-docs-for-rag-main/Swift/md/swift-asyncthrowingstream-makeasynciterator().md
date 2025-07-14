

- Swift
- AsyncThrowingStream
-  makeAsyncIterator() 

Instance Method

# makeAsyncIterator()

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func makeAsyncIterator() -> AsyncThrowingStream.Iterator
```

Available when `Failure` conforms to `Error`.

## See Also

### Creating an Iterator

struct Iterator

The asynchronous iterator for iterating an asynchronous stream.

