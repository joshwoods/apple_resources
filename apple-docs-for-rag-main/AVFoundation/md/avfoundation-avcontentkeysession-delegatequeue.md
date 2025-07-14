

- AVFoundation
- AVContentKeySession
-  delegateQueue 

Instance Property

# delegateQueue

The dispatch queue the session uses to invoke delegate callbacks.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
var delegateQueue: dispatch_queue_t? { get }
```

## See Also

### Managing the Delegate Object

func setDelegate((any AVContentKeySessionDelegate)?, queue: dispatch_queue_t?)

Sets the session’s delegate object and the dispatch queue on which to call the delegate’s methods.

var delegate: (any AVContentKeySessionDelegate)?

The content key session’s delegate object.

