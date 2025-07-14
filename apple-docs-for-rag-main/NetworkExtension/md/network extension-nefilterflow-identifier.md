

- Network Extension
- NEFilterFlow
-  identifier 

Instance Property

# identifier

The unique identifier of the flow.

iOS 13.1+iPadOS 13.1+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var identifier: UUID { get }
```

## See Also

### Inspecting flow properties

var url: URL?

The flow’s HTTP URL.

var direction: NETrafficDirection

The initial direction of the flow: incoming or outgoing.

enum NETrafficDirection

A type to represent the direction of network traffic.

var NEFilterFlowBytesMax: UInt64

The maximum number of bytes to pass or peek for a flow.

