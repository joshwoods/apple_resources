

- Network Extension
- NEFilterDataProvider
-  handleInboundData(from:readBytesStartOffset:readBytes:) 

Instance Method

# handleInboundData(from:readBytesStartOffset:readBytes:)

Make a filtering decision about a chunk of inbound data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func handleInboundData(
    from flow: NEFilterFlow,
    readBytesStartOffset offset: Int,
    readBytes: Data
) -> NEFilterDataVerdict
```

## Parameters 

`flow`  

An NEFilterFlow object containing information about the flow.

`offset`  

An unsigned integer containing the offset of the data stored in `readBytes`. This offset is measured from the beginning of the flow’s inbound data.

`readBytes`  

An NSData object containing the data to filter. For non-UDP/TCP flows, since the data may optionally include the IP header, `readBytes` includes a 4-byte NEFilterDataAttribute field preceding the user data. Your handler must examine the NEFilterDataAttribute field and handle the data accordingly.

## Return Value

A NEFilterDataVerdict object indicating how the system should handle the chunk of data and all subsequent inbound data for the flow.

## Discussion

`NEFilterDataProvider` subclasses must override this method.

## See Also

### Filtering network content

func handleNewFlow(NEFilterFlow) -> NEFilterNewFlowVerdict

Make a filtering decision for a newly-created flow of network content.

enum NEFilterDataAttribute

Attribute flags that describe the data handled by a filter.

func handleOutboundData(from: NEFilterFlow, readBytesStartOffset: Int, readBytes: Data) -> NEFilterDataVerdict

Make a filtering decision about a chunk of outbound data.

func handleInboundDataComplete(for: NEFilterFlow) -> NEFilterDataVerdict

Make a filtering decision after seeing all of the inbound data for a flow.

func handleOutboundDataComplete(for: NEFilterFlow) -> NEFilterDataVerdict

Make a filtering decision after seeing all of the outbound data for a flow.

