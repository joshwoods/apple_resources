

- Foundation
- URLSessionStreamDelegate
-  urlSession(\_:streamTask:didBecome:outputStream:) 

Instance Method

# urlSession(\_:streamTask:didBecome:outputStream:)

Tells the delegate that the stream task has been completed as a result of the stream task calling the captureStreams() method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    streamTask: URLSessionStreamTask,
    didBecome inputStream: InputStream,
    outputStream: OutputStream
)
```

## Parameters 

`session`  

The session of the stream task that has been completed.

`streamTask`  

The stream task that has been completed.

`inputStream`  

The created input stream. This InputStream object is unopened.

`outputStream`  

The created output stream. This OutputStream object is unopened

## Discussion

This delegate method will only be called after all enqueued reads and writes for the stream task have been completed.

