

- Network Extension
- NEAppProxyProvider
-  handleNewFlow(\_:) 

Instance Method

# handleNewFlow(\_:)

Handle a new flow of network data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func handleNewFlow(_ flow: NEAppProxyFlow) -> Bool
```

## Parameters 

`flow`  

The new NEAppProxyFlow object. If the App Proxy Provider decides to proxy the flow, it should create a reference to the flow in its data structures.

## Return Value

Return true to indicate that the App Proxy Provider will handle the flow. Return false to indicate that the flow should be closed.

## Mentioned in 

Handling Flow Copying

## Discussion

This method is called by the system whenever an app which matches the current App Proxy configuration’s app rules opens a new network connection.

`NEAppProxyProvider` subclasses must override this method.

New flows are initially in an unopened state. The App Proxy Provider should take whatever steps are necessary to ready itself to handle the flow data and then open the flow.

## See Also

### Handling proxied flows

func handleNewUDPFlow(NEAppProxyUDPFlow, initialRemoteEndpoint: NWEndpoint) -> Bool

Handle a new UDP flow of network data.

Deprecated

