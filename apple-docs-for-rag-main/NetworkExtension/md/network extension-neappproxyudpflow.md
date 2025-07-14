

- Network Extension
-  NEAppProxyUDPFlow 

Class

# NEAppProxyUDPFlow

An object for reading and writing data to and from a UDP conversation being proxied by the provider.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class NEAppProxyUDPFlow
```

## Mentioned in 

Handling Flow Copying

## Overview

App Proxy Providers receive UDP connections to be proxied in the form of `NEAppProxyUDPFlow` objects.

## Topics

### Handling flow data

func readDatagrams(completionHandler: ([Data]?, [NWEndpoint]?, (any Error)?) -> Void)

Read datagrams from the flow.

Deprecated

func writeDatagrams([Data], sentBy: [NWEndpoint], completionHandler: ((any Error)?) -> Void)

Write datagrams to the flow.

Deprecated

### Getting flow information

var localEndpoint: NWEndpoint?

An NWEndpoint object containing information about the local endpoint of the flow.

Deprecated

### Instance Properties

var localFlowEndpoint: NWEndpoint?

### Instance Methods

func readDatagrams() async -> ([(Data, NWEndpoint)]?, (any Error)?)

func readDatagrams(completionHandler: ([(Data, NWEndpoint)]?, (any Error)?) -> Void)

func writeDatagrams([(Data, NWEndpoint)]) async throws

func writeDatagrams([(Data, NWEndpoint)], completionHandler: ((any Error)?) -> Void)

## Relationships

### Inherits From

- NEAppProxyFlow

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

class NEAppProxyFlow

An abstract base class shared by NEAppProxyTCPFlow and NEAppProxyUDPFlow.

class NEFlowMetaData

Additional information about data flowing through a per-app VPN provider.

In-Provider Networking

Network APIs for use by all types of NetworkExtension providers and by hotspot helpers.

Handling Flow Copying

Exchange data streams by using proxy-provider classes.

