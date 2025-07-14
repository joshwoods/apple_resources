

- Network Extension
-  NEFilterDataAttribute 

Enumeration

# NEFilterDataAttribute

Attribute flags that describe the data handled by a filter.

macOS 10.15.5+

``` source
enum NEFilterDataAttribute
```

## Topics

### Attributes

case hasIPHeader

An attribute that indicates the data includes an IP header.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Filtering network content

func handleNewFlow(NEFilterFlow) -> NEFilterNewFlowVerdict

Make a filtering decision for a newly-created flow of network content.

func handleInboundData(from: NEFilterFlow, readBytesStartOffset: Int, readBytes: Data) -> NEFilterDataVerdict

Make a filtering decision about a chunk of inbound data.

func handleOutboundData(from: NEFilterFlow, readBytesStartOffset: Int, readBytes: Data) -> NEFilterDataVerdict

Make a filtering decision about a chunk of outbound data.

func handleInboundDataComplete(for: NEFilterFlow) -> NEFilterDataVerdict

Make a filtering decision after seeing all of the inbound data for a flow.

func handleOutboundDataComplete(for: NEFilterFlow) -> NEFilterDataVerdict

Make a filtering decision after seeing all of the outbound data for a flow.

