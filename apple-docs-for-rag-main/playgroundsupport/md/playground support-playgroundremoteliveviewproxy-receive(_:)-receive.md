

- Playground Support
- PlaygroundRemoteLiveViewProxy
-  receive(\_:) 

Instance Method

# receive(\_:)

Allows the proxy to receive a live view message from a remote object.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func receive(_ message: PlaygroundValue)
```

## Parameters 

`message`  

A message sent to a live view from a remote object.

## Discussion

The example below implements this method to receive a dictionary with a command from a remote object.

func receive(_ message: PlaygroundValue) {
       guard case let .dictionary(dict) = message else { return }
       guard case let .string(commandName)? = dict[&quot;command&quot;] else { return }

       // Use commandName to perform the specified command.
}

## Relationships

### From Protocol

- PlaygroundLiveViewMessageHandler

## See Also

### Receiving Messages

var delegate: PlaygroundRemoteLiveViewProxyDelegate?

A delegate you use to handle messages from the live view.

