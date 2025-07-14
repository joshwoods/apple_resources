

- UIKit
- UIResponder
-  remoteControlReceived(with:) 

Instance Method

# remoteControlReceived(with:)

Tells the object when a remote-control event is received.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func remoteControlReceived(with event: UIEvent?)
```

## Parameters 

`event`  

An event object encapsulating a remote-control command. Remote-control events have a type of UIEvent.EventType.remoteControl.

## Discussion

Remote-control events originate as commands from external accessories, including headsets. An app responds to these commands by controlling audio or video media presented to the user. The receiving responder object should examine the subtype of `event` to determine the intended command — for example, *play* (UIEvent.EventSubtype.remoteControlPlay) — and then proceed accordingly.

To allow delivery of remote-control events, you must call the beginReceivingRemoteControlEvents() method of UIApplication. To turn off delivery of remote-control events, call the endReceivingRemoteControlEvents() method.

