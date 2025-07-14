

- Playground Support
-  PlaygroundRemoteLiveViewProxy 

Class

# PlaygroundRemoteLiveViewProxy

A proxy that facilitates message passing between the always-on live view and its corresponding playground page.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
class PlaygroundRemoteLiveViewProxy
```

## Overview

Because playground pages and the always-on live view run in separate processes, you use a `PlaygroundRemoteLiveViewProxy` as a wrapper for communicating with the always-on live view.

An instance of `PlaygroundRemoteLiveViewProxy` is automatically created when you've configured the always-on live view in a playground page's `LiveView.swift` file. It's assigned as the value of `PlaygroundPage.current.liveView` only when using always-on live view. Otherwise, that property is `nil` or a local view.

guard let remoteView = PlaygroundPage.current.liveView as? PlaygroundRemoteLiveViewProxy else {
    fatalError(&quot;The always-on live view wasn&#39;t configured in this page&#39;s LiveView.swift.&quot;)
}

## Topics

### Sending Messages

func send(PlaygroundValue)

Sends a message to the always-on live view.

### Receiving Messages

var delegate: PlaygroundRemoteLiveViewProxyDelegate?

A delegate you use to handle messages from the live view.

func receive(PlaygroundValue)

Allows the proxy to receive a live view message from a remote object.

### Handling Connection Changes

func liveViewMessageConnectionOpened()

Informs the proxy that it has connected to a remote object.

func liveViewMessageConnectionClosed()

Informs the proxy that the connection between the proxy and the remote object was closed.

### Inspecting Live View Proxies

var playgroundLiveViewRepresentation: PlaygroundLiveViewRepresentation

A representation of the live view that this object is a proxy for.

Deprecated

## Relationships

### Conforms To

- PlaygroundLiveViewMessageHandler
- PlaygroundLiveViewable

## See Also

### Page-View Communication

Messaging Between a Playground Page and the Always-On Live View

Display the results of running a playground page's code in a persistent live view.

protocol PlaygroundRemoteLiveViewProxyDelegate

A delegate you use to receive messages from the always-on live view.

protocol PlaygroundLiveViewMessageHandler

A handler you use to send and receive messages between the always-on live view and its corresponding playground page.

