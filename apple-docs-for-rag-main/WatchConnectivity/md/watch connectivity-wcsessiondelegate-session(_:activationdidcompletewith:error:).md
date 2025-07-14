

- Watch Connectivity
- WCSessionDelegate
-  session(\_:activationDidCompleteWith:error:) 

Instance Method

# session(\_:activationDidCompleteWith:error:)

Tells the delegate that the session has finished activating.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.2+

``` source
func session(
    _ session: WCSession,
    activationDidCompleteWith activationState: WCSessionActivationState,
    error: (any Error)?
)
```

**Required**

## Parameters 

`session`  

The session object whose activation completed.

`activationState`  

The state of the session. Sessions normally move to the WCSessionActivationState.activated state upon success or the WCSessionActivationState.notActivated state when there is an error. On iOS, the session may also move to the WCSessionActivationState.inactive state if there is data waiting to be delivered from a previous session.

`error`  

An error object indicating that a problem occurred or `nil` if activation completed successfully. When the `activationState` parameter contains the value WCSessionActivationState.notActivated, this parameter contains the error object describing the reason for the failure.

## Discussion

You must implement this method to support asynchronous activation and quick watch switching. Your implementation should check the value of the `activationState` parameter to see if communication with the counterpart app is possible. When the state is WCSessionActivationState.activated, you may communicate normally with the other app.

## See Also

### Managing Session Activation

func sessionDidBecomeInactive(WCSession)

Tells the delegate that the session will stop communicating with the current Apple Watch.

**Required**

func sessionDidDeactivate(WCSession)

Tells the delegate that the session has delivered all the data from the previous session, and that communication with the Apple Watch has ended.

**Required**

