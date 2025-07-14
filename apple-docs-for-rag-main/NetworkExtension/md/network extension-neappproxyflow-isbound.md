

- Network Extension
- NEAppProxyFlow
-  isBound 

Instance Property

# isBound

A Boolean value that indicates whether the flow has a binding to a specific interface.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+macOS 11.1+visionOS 1.0+

``` source
var isBound: Bool { get }
```

## Discussion

When a binding exists, this value is true, and the networkInterface property indicates the bound interface. If the flow isn’t bound to an interface, this value is false.

## See Also

### Accessing flow information

var metaData: NEFlowMetaData

A metadata object containing information about the source app of the flow.

func setMetadata(nw_parameters_t)

Sets the flow’s metadata for use by proxy providers.

typealias nw_parameters_t = any OS_nw_parameters

An object that stores the protocols to use for connections, options for sending data, and network path constraints.

var networkInterface: nw_interface_t?

The network interface, if any, used by this flow.

struct nw_interface_type_t

Types of network interfaces, based on their link layer media types.

var remoteHostname: String?

The remote host name for flows created from a hostname.

