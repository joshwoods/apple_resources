

- Playground Support
- PlaygroundLiveViewMessageHandler
-  receive(\_:) 

Instance Method

# receive(\_:)

Allows the handler to receive a live view message from a remote object.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func receive(_ message: PlaygroundValue)
```

**Required** Default implementation provided.

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

## Default Implementations

### PlaygroundLiveViewMessageHandler Implementations

func receive(PlaygroundValue)

Allows the handler to receive a live view message from a remote object.

