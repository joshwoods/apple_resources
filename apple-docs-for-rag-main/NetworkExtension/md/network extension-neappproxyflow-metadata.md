

- Network Extension
- NEAppProxyFlow
-  metaData 

Instance Property

# metaData

A metadata object containing information about the source app of the flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var metaData: NEFlowMetaData { get }
```

## See Also

### Accessing flow information

func setMetadata(nw_parameters_t)

Sets the flow’s metadata for use by proxy providers.

typealias nw_parameters_t = any OS_nw_parameters

An object that stores the protocols to use for connections, options for sending data, and network path constraints.

var isBound: Bool

A Boolean value that indicates whether the flow has a binding to a specific interface.

var networkInterface: nw_interface_t?

The network interface, if any, used by this flow.

struct nw_interface_type_t

Types of network interfaces, based on their link layer media types.

var remoteHostname: String?

The remote host name for flows created from a hostname.

