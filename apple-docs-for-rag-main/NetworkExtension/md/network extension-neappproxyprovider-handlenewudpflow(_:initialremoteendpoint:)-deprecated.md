

- Network Extension
- NEAppProxyProvider
-  handleNewUDPFlow(\_:initialRemoteEndpoint:) Deprecated

Instance Method

# handleNewUDPFlow(\_:initialRemoteEndpoint:)

Handle a new UDP flow of network data.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func handleNewUDPFlow(
    _ flow: NEAppProxyUDPFlow,
    initialRemoteEndpoint remoteEndpoint: NWEndpoint
) -> Bool
```

## Parameters 

`flow`  

The new UDP flow.

`remoteEndpoint`  

The initial remote endpoint provided by the proxied app when the flow was opened.

## Discussion

The framework calls this function to deliver a new UDP data flow to the proxy provider implementation. Subclasses can override this method to perform whatever steps are necessary to ready the proxy to receive data from the flow.

If you decide to handle the flow, the subclass implementation of this method should return true. In this case, your implementation is responsible for retaining the NEAppProxyUDPFlow object.

Your implementation indicates that it’s ready to handle flow data by calling open(withLocalEndpoint:completionHandler:) on the flow.

If you decide to not handle the flow and instead terminate it, your implementation of this method should return false. This terminates the flow.

The default implementation of this method calls handleNewFlow(_:) and returns its result.

## See Also

### Handling proxied flows

func handleNewFlow(NEAppProxyFlow) -> Bool

Handle a new flow of network data.

