

- Watch Connectivity
- WCSession
-  isReachable 

Instance Property

# isReachable

A Boolean value indicating whether the counterpart app is available for live messaging.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isReachable: Bool { get }
```

## Discussion

This property is true when the WatchKit extension and the iOS app can communicate with each other.

Specifically: 

- **WatchKit extension.** The iOS device is within range, so communication can occur and the WatchKit extension is running in the foreground, or is running with a high priority in the background (for example, during a workout session or when a complication is loading its initial timeline data).

- **iOS app.** A paired and active Apple Watch is in range, the corresponding WatchKit extension is running, and the WatchKit extension’s isReachable property is true.

In all other cases, the value is false.

The counterpart must be reachable in order for you to send messages using the sendMessage(_:replyHandler:errorHandler:) and sendMessageData(_:replyHandler:errorHandler:) methods. Sending messages to a counterpart that is not reachable results in an error.

The value in this property is valid only for a configured session that has been activated successfully. If the activationState property is available, its value must be WCSessionActivationState.activated. When the session becomes inactive or deactivated, you should ignore the value in this property.

