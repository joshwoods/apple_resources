

- Network Extension
- NEFilterFlow
-  url 

Instance Property

# url

The flow’s HTTP URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var url: URL? { get }
```

## Discussion

This parameter is only non-`nil` for flows that originate from WebKit browser objects.

## See Also

### Inspecting flow properties

var identifier: UUID

The unique identifier of the flow.

var direction: NETrafficDirection

The initial direction of the flow: incoming or outgoing.

enum NETrafficDirection

A type to represent the direction of network traffic.

var NEFilterFlowBytesMax: UInt64

The maximum number of bytes to pass or peek for a flow.

