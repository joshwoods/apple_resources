

- Playground Support
-  PlaygroundRemoteLiveViewProxyDelegate 

Protocol

# PlaygroundRemoteLiveViewProxyDelegate

A delegate you use to receive messages from the always-on live view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
protocol PlaygroundRemoteLiveViewProxyDelegate : AnyObject
```

## Topics

### Receiving Messages

func remoteLiveViewProxy(PlaygroundRemoteLiveViewProxy, received: PlaygroundValue)

Tells the delegate that a message was received from the always-on live view.

**Required**

### Handling Connection Changes

func remoteLiveViewProxyConnectionClosed(PlaygroundRemoteLiveViewProxy)

Tells the delegate that it has disconnected from the always-on live view.

**Required**

## See Also

### Page-View Communication

Messaging Between a Playground Page and the Always-On Live View

Display the results of running a playground page's code in a persistent live view.

class PlaygroundRemoteLiveViewProxy

A proxy that facilitates message passing between the always-on live view and its corresponding playground page.

protocol PlaygroundLiveViewMessageHandler

A handler you use to send and receive messages between the always-on live view and its corresponding playground page.

