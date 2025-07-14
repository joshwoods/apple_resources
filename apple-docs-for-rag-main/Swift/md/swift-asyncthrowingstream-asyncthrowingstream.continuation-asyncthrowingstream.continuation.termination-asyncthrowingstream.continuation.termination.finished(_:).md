

- Swift
- AsyncThrowingStream
- AsyncThrowingStream.Continuation
- AsyncThrowingStream.Continuation.Termination
-  AsyncThrowingStream.Continuation.Termination.finished(\_:) 

Case

# AsyncThrowingStream.Continuation.Termination.finished(\_:)

The stream finished as a result of calling the continuation’s `finish` method.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case finished(Failure?)
```

## Discussion

The associated `Failure` value provides the error that terminated the stream. If no error occurred, this value is `nil`.

## See Also

### Termination States

case cancelled

The stream finished as a result of cancellation.

