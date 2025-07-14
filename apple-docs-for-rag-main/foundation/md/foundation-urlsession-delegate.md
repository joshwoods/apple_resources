

- Foundation
- URLSession
-  delegate 

Instance Property

# delegate

The delegate assigned when this object was created.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var delegate: (any URLSessionDelegate)? { get }
```

## Discussion

This delegate object is responsible for handling authentication challenges, for making caching decisions, and for handling other session-related events. The session object keeps a strong reference to this delegate until your app exits or explicitly invalidates the session. If you do not invalidate the session, your app leaks memory until it exits.

Note

This delegate object must be set at object creation time and may not be changed.

## See Also

### Working with a delegate

protocol URLSessionDelegate

A protocol that defines methods that URL session instances call on their delegates to handle session-level events, like session life cycle changes.

protocol URLSessionTaskDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events.

var delegateQueue: OperationQueue

The operation queue provided when this object was created.

