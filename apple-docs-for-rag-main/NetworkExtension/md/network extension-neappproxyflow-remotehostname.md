

- Network Extension
- NEAppProxyFlow
-  remoteHostname 

Instance Property

# remoteHostname

The remote host name for flows created from a hostname.

iOS 14.2+iPadOS 14.2+Mac Catalyst 14.2+macOS 11.0+visionOS 1.0+

``` source
var remoteHostname: String? { get }
```

## Discussion

The flow populates this property when you create the flow from a connect-by-name API such as URLSession or the Network framework.

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

var networkInterface: nw_interface_t?

The network interface, if any, used by this flow.

struct nw_interface_type_t

Types of network interfaces, based on their link layer media types.

