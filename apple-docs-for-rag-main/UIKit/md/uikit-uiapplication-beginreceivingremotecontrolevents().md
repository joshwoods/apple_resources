

- UIKit
- UIApplication
-  beginReceivingRemoteControlEvents() 

Instance Method

# beginReceivingRemoteControlEvents()

Tells the app to begin receiving remote-control events.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func beginReceivingRemoteControlEvents()
```

## Discussion

In iOS 7.1 and later, use the shared MPRemoteCommandCenter object to register for remote control events. You do not need to call this method when using the shared command center object.

This method starts the delivery of remote control events using the responder chain. Remote-control events originate as commands issued by headsets and external accessories that are intended to control multimedia presented by an app. To stop the reception of remote-control events, you must call endReceivingRemoteControlEvents().

## See Also

### Receiving remote control events

func endReceivingRemoteControlEvents()

Tells the app to stop receiving remote-control events.

