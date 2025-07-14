

- Network Extension
- NEDNSProxyProvider
-  handleNewFlow(\_:) 

Instance Method

# handleNewFlow(\_:)

Handles a new flow of DNS traffic.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func handleNewFlow(_ flow: NEAppProxyFlow) -> Bool
```

## Parameters 

`flow`  

The flow representing the DNS traffic that the proxy should handle.

## Return Value

A Boolean value set to true if the proxy implementation decides to handle the flow, or false if it instead decides to terminate the flow.

## Discussion

The system calls this method to deliver a new network data flow to the proxy provider implementation. Subclasses must override this method to perform whatever steps are necessary to ready the proxy to receive data from the flow.

The proxy provider indicates that the proxy is ready to handle flow data by calling the flow’s open(withLocalEndpoint:completionHandler:) method.

If the proxy implementation decides to handle the flow, it’s responsible for retaining a reference to the flow instance.

## See Also

### Handling proxied DNS flow

func handleNewUDPFlow(NEAppProxyUDPFlow, initialRemoteEndpoint: NWEndpoint) -> Bool

Handles a new flow of UDP traffic.

Deprecated

