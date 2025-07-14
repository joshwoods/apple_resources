

- Network Extension
-  NEAppProxyFlow 

Class

# NEAppProxyFlow

An abstract base class shared by NEAppProxyTCPFlow and NEAppProxyUDPFlow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class NEAppProxyFlow
```

## Mentioned in 

Handling Flow Copying

## Overview

App Proxy Providers receive network connections to be proxied in the form of `NEAppProxyFlow` objects, which are passed to the App Proxy Provider via the handleNewFlow(_:) method.

`NEAppProxyFlow` objects are initially in an unopened state. Before they can be used to transmit network data, they must be opened using the open(withLocalEndpoint:completionHandler:) method. When you are finished with a flow, you should call closeReadWithError(_:) and closeWriteWithError(_:), and then release the `NEAppProxyFlow` object.

## Topics

### Managing the flow life cycle

func open(withLocalEndpoint: NWHostEndpoint?, completionHandler: ((any Error)?) -> Void)

Opens the flow, indicating to the system that the caller is ready to start receiving and sending data.

Deprecated

func closeReadWithError((any Error)?)

Close the flow for further read operations.

func closeWriteWithError((any Error)?)

Close the flow for further write operations.

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

var remoteHostname: String?

The remote host name for flows created from a hostname.

### Errors

struct NEAppProxyFlowError

An error that the app proxy flow encounters.

let NEAppProxyErrorDomain: String

The domain used for app proxy errors.

enum Code

Error codes that the app proxy flow API declares.

struct NEAppProxyFlowError

An error that the app proxy flow encounters.

### Instance Properties

var interface: NWInterface?

### Instance Methods

func open(withLocalFlowEndpoint: NWEndpoint?) async throws

func open(withLocalFlowEndpoint: NWEndpoint?, completionHandler: ((any Error)?) -> Void)

func setMetadata(on: NWParameters)

## Relationships

### Inherits From

- NSObject

### Inherited By

- NEAppProxyTCPFlow
- NEAppProxyUDPFlow

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Flow handling

class NEAppProxyTCPFlow

An object for reading and writing data to and from a TCP connection being proxied by the provider.

class NEAppProxyUDPFlow

An object for reading and writing data to and from a UDP conversation being proxied by the provider.

class NEFlowMetaData

Additional information about data flowing through a per-app VPN provider.

In-Provider Networking

Network APIs for use by all types of NetworkExtension providers and by hotspot helpers.

Handling Flow Copying

Exchange data streams by using proxy-provider classes.

