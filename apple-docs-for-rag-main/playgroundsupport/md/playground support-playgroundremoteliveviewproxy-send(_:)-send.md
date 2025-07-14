

- Playground Support
- PlaygroundRemoteLiveViewProxy
-  send(\_:) 

Instance Method

# send(\_:)

Sends a message to the always-on live view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func send(_ message: PlaygroundValue)
```

## Parameters 

`message`  

A message to send to a remote object.

## Discussion

Calling this method requires an open connection to a remote object.

