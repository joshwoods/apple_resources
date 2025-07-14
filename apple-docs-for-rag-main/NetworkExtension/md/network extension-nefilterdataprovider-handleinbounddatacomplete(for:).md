

- Network Extension
- NEFilterDataProvider
-  handleInboundDataComplete(for:) 

Instance Method

# handleInboundDataComplete(for:)

Make a filtering decision after seeing all of the inbound data for a flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func handleInboundDataComplete(for flow: NEFilterFlow) -> NEFilterDataVerdict
```

## Parameters 

`flow`  

An NEFilterFlow object containing information about the flow.

## Return Value

An NEFilterDataVerdict object indicating how the system should handle the flow of network content.

## Discussion

The system calls this method after all of the inbound data for a flow of network content has been given to the Filter Data Provider.

`NEFilterDataProvider` subclasses must override this method.

## See Also

### Filtering network content

func handleNewFlow(NEFilterFlow) -> NEFilterNewFlowVerdict

Make a filtering decision for a newly-created flow of network content.

func handleInboundData(from: NEFilterFlow, readBytesStartOffset: Int, readBytes: Data) -> NEFilterDataVerdict

Make a filtering decision about a chunk of inbound data.

enum NEFilterDataAttribute

Attribute flags that describe the data handled by a filter.

func handleOutboundData(from: NEFilterFlow, readBytesStartOffset: Int, readBytes: Data) -> NEFilterDataVerdict

Make a filtering decision about a chunk of outbound data.

func handleOutboundDataComplete(for: NEFilterFlow) -> NEFilterDataVerdict

Make a filtering decision after seeing all of the outbound data for a flow.

