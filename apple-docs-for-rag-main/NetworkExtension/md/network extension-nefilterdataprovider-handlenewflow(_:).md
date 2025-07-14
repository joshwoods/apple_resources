

- Network Extension
- NEFilterDataProvider
-  handleNewFlow(\_:) 

Instance Method

# handleNewFlow(\_:)

Make a filtering decision for a newly-created flow of network content.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func handleNewFlow(_ flow: NEFilterFlow) -> NEFilterNewFlowVerdict
```

## Parameters 

`flow`  

An NEFilterFlow object containing information about the new flow.

## Return Value

An NEFilterNewFlowVerdict object indicating how the system should handle the flow.

## Discussion

This function is called by the system when a filtering decision needs to be made about a new flow of network content.

`NEFilterDataProvider` subclasses must override this method.

## See Also

### Filtering network content

func handleInboundData(from: NEFilterFlow, readBytesStartOffset: Int, readBytes: Data) -> NEFilterDataVerdict

Make a filtering decision about a chunk of inbound data.

enum NEFilterDataAttribute

Attribute flags that describe the data handled by a filter.

func handleOutboundData(from: NEFilterFlow, readBytesStartOffset: Int, readBytes: Data) -> NEFilterDataVerdict

Make a filtering decision about a chunk of outbound data.

func handleInboundDataComplete(for: NEFilterFlow) -> NEFilterDataVerdict

Make a filtering decision after seeing all of the inbound data for a flow.

func handleOutboundDataComplete(for: NEFilterFlow) -> NEFilterDataVerdict

Make a filtering decision after seeing all of the outbound data for a flow.

