

- Swift
- AsyncStream
- AsyncStream.Iterator
-  next() 

Instance Method

# next()

The next value from the asynchronous stream.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func next() async -> Element?
```

## Discussion

When `next()` returns `nil`, this signifies the end of the `AsyncStream`.

It is a programmer error to invoke `next()` from a concurrent context that contends with another such call, which results in a call to `fatalError()`.

If you cancel the task this iterator is running in while `next()` is awaiting a value, the `AsyncStream` terminates. In this case, `next()` might return `nil` immediately, or return `nil` on subsequent calls.

