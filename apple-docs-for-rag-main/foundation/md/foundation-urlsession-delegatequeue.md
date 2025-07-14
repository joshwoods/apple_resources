

- Foundation
- URLSession
-  delegateQueue 

Instance Property

# delegateQueue

The operation queue provided when this object was created.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var delegateQueue: OperationQueue { get }
```

## Mentioned in 

Processing URL session data task results with Combine

## Discussion

All delegate method calls and completion handlers related to the session are performed on this queue. The session object keeps a strong reference to this queue until your app exits or the session object is deallocated. If you do not invalidate the session, your app leaks memory until it exits.

Note

This queue must be set at object creation time and may not be changed.

## See Also

### Working with a delegate

var delegate: (any URLSessionDelegate)?

The delegate assigned when this object was created.

protocol URLSessionDelegate

A protocol that defines methods that URL session instances call on their delegates to handle session-level events, like session life cycle changes.

protocol URLSessionTaskDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events.

