

- Watch Connectivity
- WCSession
-  activationState 

Instance Property

# activationState

The current activation state of the session.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.2+

``` source
var activationState: WCSessionActivationState { get }
```

## Discussion

Check the value of this property before attempting to transfer data or files using the methods of this object. When the value is WCSessionActivationState.activated you may initiate the transfer of data and files normally. If it is any other value, do not initiate any transfers.

The value of this property is valid even when the session itself is not activated, so you can access it at any time. Use the sessionDidBecomeInactive(_:) and sessionDidDeactivate(_:) methods of your session delegate to monitor changes in the session’s activation state. You can also use key-value observing to monitor changes to this property.

## See Also

### Configuring the Session

var delegate: (any WCSessionDelegate)?

The delegate for the session object

func activate()

Activates the session asynchronously.

