

- UIKit
- UIApplication
-  endReceivingRemoteControlEvents() 

Instance Method

# endReceivingRemoteControlEvents()

Tells the app to stop receiving remote-control events.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func endReceivingRemoteControlEvents()
```

## Discussion

In iOS 7.1 and later, use the shared MPRemoteCommandCenter object to unregister for remote control events. You do not need to call this method when using the shared command center object.

This method stops the delivery of remote control events using the responder chain. Remote-control events originate as commands issued by headsets and external accessories that are intended to control multimedia presented by an app.

## See Also

### Receiving remote control events

func beginReceivingRemoteControlEvents()

Tells the app to begin receiving remote-control events.

