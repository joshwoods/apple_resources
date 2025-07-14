

- Network Extension
- NEAppProxyUDPFlow
-  readDatagrams(completionHandler:) Deprecated

Instance Method

# readDatagrams(completionHandler:)

Read datagrams from the flow.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func readDatagrams(completionHandler: @escaping ([Data]?, [NWEndpoint]?, (any Error)?) -> Void)
```

## Parameters 

`completionHandler`  

A block that will be executed by the system on an internal system thread when datagrams have been read from the flow. The block takes the datagrams that were read, the destination endpoints of the datagrams, and an NSError. If an error occurred while reading then `error` will be non-nil. See `NEAppProxyFlowError` in NEAppProxyFlow for a list of possible error codes. If the `datagrams` and `remoteEndpoints` arrays are non-nil but are empty, then no more datagrams can be subsequently read from the flow.

Note

The completion handler is only called for the single read operation that was initiated by calling this method. If the caller wants to read more datagrams then it should call this method again to schedule another read operation and another execution of the completion handler block.

## See Also

### Handling flow data

func writeDatagrams([Data], sentBy: [NWEndpoint], completionHandler: ((any Error)?) -> Void)

Write datagrams to the flow.

Deprecated

