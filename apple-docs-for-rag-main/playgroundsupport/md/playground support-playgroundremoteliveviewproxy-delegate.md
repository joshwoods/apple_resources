

- Playground Support
- PlaygroundRemoteLiveViewProxy
-  delegate 

Instance Property

# delegate

A delegate you use to handle messages from the live view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
weak var delegate: PlaygroundRemoteLiveViewProxyDelegate?
```

## See Also

### Receiving Messages

func receive(PlaygroundValue)

Allows the proxy to receive a live view message from a remote object.

