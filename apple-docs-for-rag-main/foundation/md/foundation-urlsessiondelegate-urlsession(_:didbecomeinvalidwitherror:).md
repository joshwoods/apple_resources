

- Foundation
- URLSessionDelegate
-  urlSession(\_:didBecomeInvalidWithError:) 

Instance Method

# urlSession(\_:didBecomeInvalidWithError:)

Tells the URL session that the session has been invalidated.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    didBecomeInvalidWithError error: (any Error)?
)
```

## Parameters 

`session`  

The session object that was invalidated.

`error`  

The error that caused invalidation, or `nil` if the invalidation was explicit.

## Discussion

If you invalidate a session by calling its finishTasksAndInvalidate() method, the session waits until after the final task in the session finishes or fails before calling this delegate method. If you call the invalidateAndCancel() method, the session calls this delegate method immediately.

## See Also

### Handling session life cycle changes

func urlSessionDidFinishEvents(forBackgroundURLSession: URLSession)

Tells the delegate that all messages enqueued for a session have been delivered.

