

- Watch Connectivity
- WCSessionDelegate
-  sessionWatchStateDidChange(\_:) 

Instance Method

# sessionWatchStateDidChange(\_:)

Indicates a change to the counterpart’s information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
optional func sessionWatchStateDidChange(_ session: WCSession)
```

## Parameters 

`session`  

The session object whose state changed.

## Discussion

The session object calls this method when the value in the isPaired, isWatchAppInstalled, isComplicationEnabled, or watchDirectoryURL properties of the WCSession object changes. Use this state to update the state of your iOS app. For example, when the complication is disabled, make a note of that fact and do not send any more data updates for the complication.

## See Also

### Managing State Changes

func sessionReachabilityDidChange(WCSession)

Indicates a change to the counterpart’s reachability status.

func sessionCompanionAppInstalledDidChange(WCSession)

Indicates a change to the companion app’s installed state.

