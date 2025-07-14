

- Network Extension
- App proxy provider
-  In-Provider Networking 

API Collection

# In-Provider Networking

Network APIs for use by all types of NetworkExtension providers and by hotspot helpers.

## Overview

NetworkExtension providers and hotspot helpers run in an unusual network environment that can cause problems for general-purpose networking APIs. For example, URLSession typically sends requests via the default route, which is inappropriate for a hotspot helper that must always use the Wi-Fi interface. The NetworkExtension framework includes a number of APIs that are useful in such situations.

These APIs have the following key characteristics:

- They aren’t general-purpose APIs; they can only be used in the context of a NetworkExtension provider or hotspot helper.

- In many cases, you don’t need to use them. For example, it’s possible for a packet tunnel provider to use a general-purpose networking API, like BSD Sockets, for its tunnel connection.

The recommended general-purpose networking APIs are the URL Loading System for HTTP and the Network framework for TCP and UDP.

## Topics

### TCP connections

class NWTCPConnection

An object to manage a TCP connection, with or without TLS.

Deprecated

class NWTLSParameters

TLS properties for creating a connection.

Deprecated

protocol NWTCPConnectionAuthenticationDelegate

A delegate protocol to customize the TLS authentication done by a connection.

Deprecated

### UDP sessions

class NWUDPSession

An object to manage a UDP session to a network endpoint.

Deprecated

### Endpoints

class NWHostEndpoint

A network endpoint specified by DNS name (or IP address) and port.

Deprecated

class NWBonjourServiceEndpoint

A network endpoint specified as a Bonjour service name, type, and domain.

Deprecated

class NWEndpoint

An abstract base class, shared by NWHostEndpoint or NWBonjourServiceEndpoint, that represents the source or destination of a network connection.

Deprecated

### Network path information

class NWPath

The path made by a network connection, including information about its viability.

Deprecated

## See Also

### Related Documentation

Packet tunnel provider

Implement a VPN client for a packet-oriented, custom VPN protocol.

App proxy provider

Implement a VPN client for a flow-oriented, custom VPN protocol.

Hotspot helper

Integrate your app with the iOS hotspot network subsystem.

### Flow handling

class NEAppProxyTCPFlow

An object for reading and writing data to and from a TCP connection being proxied by the provider.

class NEAppProxyUDPFlow

An object for reading and writing data to and from a UDP conversation being proxied by the provider.

class NEAppProxyFlow

An abstract base class shared by NEAppProxyTCPFlow and NEAppProxyUDPFlow.

class NEFlowMetaData

Additional information about data flowing through a per-app VPN provider.

Handling Flow Copying

Exchange data streams by using proxy-provider classes.

