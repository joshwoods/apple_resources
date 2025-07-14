

- Network Extension
- NEAppProxyFlow
-  networkInterface 

Instance Property

# networkInterface

The network interface, if any, used by this flow.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS 1.0+

``` source
@NSCopying
var networkInterface: nw_interface_t? { get set }
```

## Discussion

To transport the flow’s data over a different interface, set this property to that interface.

## See Also

### Accessing flow information

var metaData: NEFlowMetaData

A metadata object containing information about the source app of the flow.

func setMetadata(nw_parameters_t)

Sets the flow’s metadata for use by proxy providers.

typealias nw_parameters_t = any OS_nw_parameters

An object that stores the protocols to use for connections, options for sending data, and network path constraints.

var isBound: Bool

A Boolean value that indicates whether the flow has a binding to a specific interface.

struct nw_interface_type_t

Types of network interfaces, based on their link layer media types.

var remoteHostname: String?

The remote host name for flows created from a hostname.

