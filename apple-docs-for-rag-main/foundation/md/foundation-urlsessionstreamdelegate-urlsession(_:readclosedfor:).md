

- Foundation
- URLSessionStreamDelegate
-  urlSession(\_:readClosedFor:) 

Instance Method

# urlSession(\_:readClosedFor:)

Tells the delegate that the read side of the underlying socket has been closed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    readClosedFor streamTask: URLSessionStreamTask
)
```

## Parameters 

`session`  

The session containing the stream task that closed reads.

`streamTask`  

The stream task that closed reads.

## Discussion

This method may be called even if no reads are currently in progress. This method does not indicate that the stream reached end-of-file (EOF), such that no more data can be read.

## See Also

### Handling closing events

func urlSession(URLSession, writeClosedFor: URLSessionStreamTask)

Tells the delegate that the write side of the underlying socket has been closed.

