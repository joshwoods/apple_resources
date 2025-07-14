

- Watch Connectivity
- WCSession
-  delegate 

Instance Property

# delegate

The delegate for the session object

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any WCSessionDelegate)? { get set }
```

## Discussion

You must assign an object conforming to the WCSessionDelegate protocol to this property before calling the activate() method. The delegate is responsible for responding to session-related changes, for processing incoming data, and for responding to errors.

For more information about implementing your delegate object, see WCSessionDelegate.

## See Also

### Configuring the Session

func activate()

Activates the session asynchronously.

var activationState: WCSessionActivationState

The current activation state of the session.

