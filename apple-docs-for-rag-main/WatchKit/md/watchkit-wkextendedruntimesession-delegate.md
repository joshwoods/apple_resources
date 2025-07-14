

- WatchKit
- WKExtendedRuntimeSession
-  delegate 

Instance Property

# delegate

A delegate object for monitoring the session and responding to state changes and errors.

watchOS 6.0+

``` source
weak var delegate: (any WKExtendedRuntimeSessionDelegate)? { get set }
```

## Discussion

To receive all the delegate calls, always assign a value to this property before calling the session’s start() or start(at:) methods.

## See Also

### Creating a Session

protocol WKExtendedRuntimeSessionDelegate

A set of optional methods for monitoring an extended runtime session.

