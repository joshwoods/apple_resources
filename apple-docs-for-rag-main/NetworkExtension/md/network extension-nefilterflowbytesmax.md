

- Network Extension
-  NEFilterFlowBytesMax 

Global Variable

# NEFilterFlowBytesMax

The maximum number of bytes to pass or peek for a flow.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var NEFilterFlowBytesMax: UInt64 { get }
```

## Discussion

When used as a pass value, this value directs to flow to pass all upcoming bytes. When used as a peek value, it indicates the flow should peek as many bytes as possible.

## See Also

### Inspecting flow properties

var url: URL?

The flow’s HTTP URL.

var identifier: UUID

The unique identifier of the flow.

var direction: NETrafficDirection

The initial direction of the flow: incoming or outgoing.

enum NETrafficDirection

A type to represent the direction of network traffic.

