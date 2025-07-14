

- Network Extension
- NEAppProxyFlow
-  open(withLocalEndpoint:completionHandler:) Deprecated

Instance Method

# open(withLocalEndpoint:completionHandler:)

Opens the flow, indicating to the system that the caller is ready to start receiving and sending data.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func open(
    withLocalEndpoint localEndpoint: NWHostEndpoint?,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func open(withLocalEndpoint localEndpoint: NWHostEndpoint?) async throws
```

## Parameters 

`localEndpoint`  

An NWHostEndpoint object that contains the address and port to set as the local address and local port of the flow.

The system supplies this information to the app that triggered the creation of this flow in different ways, depending on the networking API the app used. For example, if the app used the Network framework, it gets this information from the localEndpoint property of the current path. If it used BSD Sockets, it gets this information by calling `getsockname`.

Pass `nil` to have the system derive a value based on the address of the current primary physical interface.

`completionHandler`  

Called when the open operation is complete. This block has no return value and takes the following parameter:

error  
A `nil` value indicates the flow opened successfully. A non-`nil` value indicates the flow could not be opened. See NEAppProxyFlowError for a list of expected error codes.

## Discussion

An NEAppProxyFlow object starts out in the unopened state. When the system passes a flow to your app proxy provider by calling handleNewFlow(_:), to need to set up the state necessary to handle the flow’s data, and then call this method.

## See Also

### Managing the flow life cycle

func closeReadWithError((any Error)?)

Close the flow for further read operations.

func closeWriteWithError((any Error)?)

Close the flow for further write operations.

