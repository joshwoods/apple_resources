

- WatchKit
- WKExtendedRuntimeSession
-  notifyUser(hapticType:repeatHandler:) 

Instance Method

# notifyUser(hapticType:repeatHandler:)

Play a repeating haptic alert.

watchOS 6.0+

``` source
func notifyUser(
    hapticType type: WKHapticType,
    repeatHandler: ((UnsafeMutablePointer) -> TimeInterval)? = nil
)
```

## Parameters 

`type`  

The type of haptic to play. For a complete list of haptic types, see WKHapticType.

`repeatHandler`  

An optional block that the system calls to set the frequency of the haptic feedback. The handler returns a valid time interval for the next haptic signal. This value must be greater than `0.0` and less than or equal to `60.0`. If `repeatHandler` is `nil`, the system uses the default time interval of `3.0` seconds.

Use this block to change the haptic type by modifying the `outHapticType` parameter.

`outHapticType`  
The next haptic. Set the value of this output parameter to change the haptic type.

## Mentioned in 

Using extended runtime sessions

## Discussion

For schedulable sessions such as smart alarms, call this method during the session to alert the user. When you call the method, the system plays repeating haptic feedback. If the app isn’t active, the system also displays a system alarm alert on the watch.

The haptic feedback repeats at the interval specified by the `repeatHandler`, and continues to repeat until the application or system alert invalidates the session.

- If the app isn’t active, the user can tap the Stop button to invalidate the session or tap the Open button to activate the app.

- If the app is active, the app must invalidate the session by calling its invalidate() method.

Only call this method on a schedulable session that’s running: you must schedule the session using the start(at:) method, and the session’s state must equal WKExtendedRuntimeSessionState.running. During a smart alarm session, your app must call this method before the session expires.

