

- Watch Connectivity
- WCError
- WCError.Code
-  WCError.Code.sessionInactive 

Case

# WCError.Code.sessionInactive

An error indicating that the session is inactive.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.2+

``` source
case sessionInactive
```

## Discussion

This error occurs when you try to send data using an inactive session.

## See Also

### Error Codes

case genericError

An error that occurs when there is an unknown problem.

case sessionNotSupported

An error indicating that the current device doesn’t support the use of session objects.

case sessionMissingDelegate

An error indicating that the WatchKit extension doesn’t have a valid extension delegate to process events.

case sessionNotActivated

An error indicating that the other device doesn’t have an active session.

case deviceNotPaired

An error indicating that the current device doesn’t have a paired counterpart.

case watchAppNotInstalled

An error indicating that the Watch app isn’t an installed app on the user’s Apple Watch.

case notReachable

An error indicating that the counterpart app isn’t reachable.

case invalidParameter

An error indicating that a parameter is invalid.

case payloadTooLarge

An error indicating an attempt to send an item that exceeds the maximum size limit.

case payloadUnsupportedTypes

An error indicating that a dictionary contains nonproperty list types.

case messageReplyFailed

An error that occurs when the system can’t return the reply.

case messageReplyTimedOut

An error that occurs when the counterpart app doesn’t return a reply in time.

case fileAccessDenied

An error indicating that the system can’t transfer a file because it is inaccessible.

case deliveryFailed

An error that occurs when the system can’t deliver the payload.

case insufficientSpace

An error indicating that there isn’t enough space on the receiving side to store the data.

