

- Foundation
- URLSessionStreamDelegate
-  urlSession(\_:writeClosedFor:) 

Instance Method

# urlSession(\_:writeClosedFor:)

Tells the delegate that the write side of the underlying socket has been closed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    writeClosedFor streamTask: URLSessionStreamTask
)
```

## Parameters 

`session`  

The session containing the stream task that closed writes.

`streamTask`  

The stream task that closed writes.

## Discussion

This method may be called even if no writes are currently in progress.

## See Also

### Handling closing events

func urlSession(URLSession, readClosedFor: URLSessionStreamTask)

Tells the delegate that the read side of the underlying socket has been closed.

