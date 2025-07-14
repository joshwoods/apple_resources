

- Watch Connectivity
- WCSessionDelegate
-  sessionCompanionAppInstalledDidChange(\_:) 

Instance Method

# sessionCompanionAppInstalledDidChange(\_:)

Indicates a change to the companion app’s installed state.

watchOS 6.0+

``` source
optional func sessionCompanionAppInstalledDidChange(_ session: WCSession)
```

## Parameters 

`session`  

The session object with the changed companion app.

## Discussion

The system calls this method on the watchOS app’s session delegate when the user installs or uninstalls the iOS companion app. This is only valid on independent watchOS apps.

## See Also

### Managing State Changes

func sessionWatchStateDidChange(WCSession)

Indicates a change to the counterpart’s information.

func sessionReachabilityDidChange(WCSession)

Indicates a change to the counterpart’s reachability status.

