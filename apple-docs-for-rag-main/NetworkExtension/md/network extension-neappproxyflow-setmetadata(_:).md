

- Network Extension
- NEAppProxyFlow
-  setMetadata(\_:) 

Instance Method

# setMetadata(\_:)

Sets the flow’s metadata for use by proxy providers.

macOS 10.15.4+

``` source
func setMetadata(_ parameters: nw_parameters_t)
```

## Parameters 

`parameters`  

A nw_parameters_t object that contains the flow metadata.

## Discussion

Use an nw_parameters_t object to create a connection that transparently proxies the flow’s data. This also provides accurate source app information to any subsequent NEAppProxyProvider instances that transparently proxy the flow.

## See Also

### Accessing flow information

var metaData: NEFlowMetaData

A metadata object containing information about the source app of the flow.

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

