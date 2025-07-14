

- Swift
- AsyncStream
-  makeStream(of:bufferingPolicy:) 

Type Method

# makeStream(of:bufferingPolicy:)

Initializes a new AsyncStream and an AsyncStream.Continuation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@backDeployed(before: macOS 14.0, iOS 17.0, watchOS 10.0, tvOS 17.0)
static func makeStream(
    of elementType: Element.Type = Element.self,
    bufferingPolicy limit: AsyncStream.Continuation.BufferingPolicy = .unbounded
) -> (stream: AsyncStream, continuation: AsyncStream.Continuation)
```

## Parameters 

`elementType`  

The element type of the stream.

`limit`  

The buffering policy that the stream should use.

## Return Value

A tuple containing the stream and its continuation. The continuation should be passed to the producer while the stream should be passed to the consumer.

