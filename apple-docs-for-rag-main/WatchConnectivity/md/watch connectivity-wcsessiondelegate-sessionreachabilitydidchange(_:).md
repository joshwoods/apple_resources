

- Watch Connectivity
- WCSessionDelegate
-  sessionReachabilityDidChange(\_:) 

Instance Method

# sessionReachabilityDidChange(\_:)

Indicates a change to the counterpart’s reachability status.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 2.0+

``` source
optional func sessionReachabilityDidChange(_ session: WCSession)
```

## Parameters 

`session`  

The session object of the current process. Use the isReachable property of this object to determine the reachability of the counterpart session.

## Discussion

A session is reachable when the iOS app or WatchKit extension to which it belongs is active and running. This method is called to let the current process know that its counterpart session’s reachability changed. Use that information to make decisions about how you want to send information to the counterpart. For example, when the counterpart is reachable, you might send messages immediately rather than post them as an update.

## See Also

### Managing State Changes

func sessionWatchStateDidChange(WCSession)

Indicates a change to the counterpart’s information.

func sessionCompanionAppInstalledDidChange(WCSession)

Indicates a change to the companion app’s installed state.

