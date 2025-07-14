

- Playground Support
-  Messaging Between a Playground Page and the Always-On Live View 

Article

# Messaging Between a Playground Page and the Always-On Live View

Display the results of running a playground page's code in a persistent live view.

## Overview

The always-on live view in Swift Playgrounds runs continuously as learners write and debug the code in the accompanying playground page. Because the code in the playground page may change continuously, the code you write for the always-on live view runs in a separate process so it isn't continuously restarting.

Instances in a playground page can't communicate directly with instances in the always-on live view. Instead, you communicate asynchronously between the two parts of a playground by adopting a message-handling protocol and setting a delegate for a proxy object that mediates between the two processes.

### Configure the Always-On Live View

You create the always-on live view by assigning a view or view controller to the global liveView for the current page.

Important

You invoke the always-on live view from a file named `LiveView.swift`, which must be located in the directory for each playground page. If you assign the current `liveView` from any other code, the resulting live view will be a traditional live view that doesn't persist across multiple runs of the page.

Configure your always-on live view to adopt the PlaygroundLiveViewMessageHandler protocol for sending and receiving messages from the corresponding playground page. The example below uses a UIButton as the root view and changes the background color of the button when it receives a message.

### Configure the Playground Page

The always-on live view that you configure in `LiveView.swift` is visible to learner-facing code—code invoked from `main.swift`—as an instance of PlaygroundRemoteLiveViewProxy. To receive messages from the always-on live view, you define a class to be that proxy's delegate.

The example below defines a delegate for the always-on live view proxy and configures it to print any messages it receives.

### Send and Receive Messages

You send messages to the always-on live view by calling the send(_:) method on its proxy.

You send messages back to the playground page from the always-on live view by calling the send(_:) method on the view itself.

The example below builds on the example in Configure the Always-On Live View by sending a message back to the playground page in response to any messages the always-on live view receives.

## See Also

### Page-View Communication

class PlaygroundRemoteLiveViewProxy

A proxy that facilitates message passing between the always-on live view and its corresponding playground page.

protocol PlaygroundRemoteLiveViewProxyDelegate

A delegate you use to receive messages from the always-on live view.

protocol PlaygroundLiveViewMessageHandler

A handler you use to send and receive messages between the always-on live view and its corresponding playground page.

### Related Documentation

class PlaygroundPage

An object you use to configure the state of a playground page and its live view.

