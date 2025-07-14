

- Network Extension
- NEAppProxyUDPFlow
-  writeDatagrams(\_:sentBy:completionHandler:) Deprecated

Instance Method

# writeDatagrams(\_:sentBy:completionHandler:)

Write datagrams to the flow.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func writeDatagrams(
    _ datagrams: [Data],
    sentBy remoteEndpoints: [NWEndpoint],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func writeDatagrams(
    _ datagrams: [Data],
    sentBy remoteEndpoints: [NWEndpoint]
) async throws
```

## Parameters 

`datagrams`  

An array of NSData objects containing datagram payloads to be written.

`remoteEndpoints`  

An array of NWEndpoint objects containing the source endpoints of the datagram payloads in `datagrams`.

`completionHandler`  

A block that will be executed by the system on an internal system thread when the data is written into the receive buffer of the socket associated with the flow. If an error occurs while writing the data then a non-nil NSError object is passed to the block. See `NEAppProxyFlowError` in NEAppProxyFlow for a list of possible errors.

## See Also

### Handling flow data

func readDatagrams(completionHandler: ([Data]?, [NWEndpoint]?, (any Error)?) -> Void)

Read datagrams from the flow.

Deprecated

