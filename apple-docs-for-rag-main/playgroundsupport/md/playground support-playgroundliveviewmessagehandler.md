

- Playground Support
-  PlaygroundLiveViewMessageHandler 

Protocol

# PlaygroundLiveViewMessageHandler

A handler you use to send and receive messages between the always-on live view and its corresponding playground page.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
protocol PlaygroundLiveViewMessageHandler : AnyObject
```

## Topics

### Sending Messages

func send(PlaygroundValue)

Allows the handler to send a message to a remote object.

### Receiving Messages

func receive(PlaygroundValue)

Allows the handler to receive a live view message from a remote object.

**Required** Default implementation provided.

### Handling Connection Changes

func liveViewMessageConnectionOpened()

Informs the handler that it has connected to a remote object.

**Required** Default implementation provided.

func liveViewMessageConnectionClosed()

Informs the handler that the connection between the proxy and the remote object was closed.

**Required** Default implementation provided.

## Relationships

### Conforming Types

- PlaygroundRemoteLiveViewProxy

## See Also

### Page-View Communication

Messaging Between a Playground Page and the Always-On Live View

Display the results of running a playground page's code in a persistent live view.

class PlaygroundRemoteLiveViewProxy

A proxy that facilitates message passing between the always-on live view and its corresponding playground page.

protocol PlaygroundRemoteLiveViewProxyDelegate

A delegate you use to receive messages from the always-on live view.

