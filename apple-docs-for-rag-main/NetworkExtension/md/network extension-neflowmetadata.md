

- Network Extension
-  NEFlowMetaData 

Class

# NEFlowMetaData

Additional information about data flowing through a per-app VPN provider.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class NEFlowMetaData
```

## Overview

This metadata is only present for data flowing through per-app VPN providers, that is, app proxy providers and packet tunnel providers in per-app VPN mode, as indicated by the routingMethod property.

## Topics

### Getting source app information

var sourceAppUniqueIdentifier: Data

A data instance that contains a unique hash value for the source application.

var sourceAppSigningIdentifier: String

A string that contains the signing identifier of the source application.

var sourceAppAuditToken: Data?

The audit token of the source application of the flow.

### Getting flow information

var filterFlowIdentifier: UUID?

The identifier of the content filter flow corresponding to this flow.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Related Documentation

class NEPacket

A network packet and its associated properties.

### Flow handling

class NEAppProxyTCPFlow

An object for reading and writing data to and from a TCP connection being proxied by the provider.

class NEAppProxyUDPFlow

An object for reading and writing data to and from a UDP conversation being proxied by the provider.

class NEAppProxyFlow

An abstract base class shared by NEAppProxyTCPFlow and NEAppProxyUDPFlow.

In-Provider Networking

Network APIs for use by all types of NetworkExtension providers and by hotspot helpers.

Handling Flow Copying

Exchange data streams by using proxy-provider classes.

