

- Network Extension
- NEFilterFlow
-  direction 

Instance Property

# direction

The initial direction of the flow: incoming or outgoing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var direction: NETrafficDirection { get }
```

## See Also

### Inspecting flow properties

var url: URL?

The flow’s HTTP URL.

var identifier: UUID

The unique identifier of the flow.

enum NETrafficDirection

A type to represent the direction of network traffic.

var NEFilterFlowBytesMax: UInt64

The maximum number of bytes to pass or peek for a flow.

