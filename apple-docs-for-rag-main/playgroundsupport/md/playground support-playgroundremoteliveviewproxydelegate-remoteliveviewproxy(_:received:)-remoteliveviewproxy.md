

- Playground Support
- PlaygroundRemoteLiveViewProxyDelegate
-  remoteLiveViewProxy(\_:received:) 

Instance Method

# remoteLiveViewProxy(\_:received:)

Tells the delegate that a message was received from the always-on live view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func remoteLiveViewProxy(
    _ remoteLiveViewProxy: PlaygroundRemoteLiveViewProxy,
    received message: PlaygroundValue
)
```

**Required**

## Parameters 

`remoteLiveViewProxy`  

The local proxy for the remote always-on live view.

`message`  

A message sent to the playground page from the always-on live view.

