

- Network Extension
-  NEAppProxyTCPFlow 

Class

# NEAppProxyTCPFlow

An object for reading and writing data to and from a TCP connection being proxied by the provider.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class NEAppProxyTCPFlow
```

## Mentioned in 

Handling Flow Copying

## Overview

App Proxy Providers receive TCP connections to be proxied in the form of `NEAppProxyTCPFlow` objects.

## Topics

### Handling flow data

func write(Data, withCompletionHandler: ((any Error)?) -> Void)

Write data to the flow.

func readData(completionHandler: (Data?, (any Error)?) -> Void)

Read data from the flow.

### Getting flow information

var remoteEndpoint: NWEndpoint

An NWEndpoint object containing information about the intended remote endpoint of the flow.

Deprecated

### Instance Properties

var remoteFlowEndpoint: NWEndpoint

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

class NEAppProxyUDPFlow

An object for reading and writing data to and from a UDP conversation being proxied by the provider.

class NEAppProxyFlow

An abstract base class shared by NEAppProxyTCPFlow and NEAppProxyUDPFlow.

class NEFlowMetaData

Additional information about data flowing through a per-app VPN provider.

In-Provider Networking

Network APIs for use by all types of NetworkExtension providers and by hotspot helpers.

Handling Flow Copying

Exchange data streams by using proxy-provider classes.

