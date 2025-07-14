

- Network
- ProxyConfiguration
-  ProxyConfiguration.RelayHop 

Structure

# ProxyConfiguration.RelayHop

A single relay server you can chain together with other servers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct RelayHop
```

## Overview

Relay servers are secure HTTP proxies that allow proxying TCP traffic using the `CONNECT` method and UDP traffic using the `connect-udp` protocol defined in RFC 9298.

## Topics

### Creating Relay Hops

init(http3RelayEndpoint: NWEndpoint, http2RelayEndpoint: NWEndpoint?, tlsOptions: NWProtocolTLS.Options, additionalHTTPHeaderFields: [String : String])

Creates a configuration for a secure relay accessible using HTTP/3, with an optional HTTP/2 fallback.

init(http2RelayEndpoint: NWEndpoint, tlsOptions: NWProtocolTLS.Options, additionalHTTPHeaderFields: [String : String])

Creates a configuration for a secure relay accessible only using HTTP/2.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Creating Proxy Configurations

init(relayHops: [ProxyConfiguration.RelayHop])

Initializes a proxy configuration with one or two relay hops.

init(httpCONNECTProxy: NWEndpoint, tlsOptions: NWProtocolTLS.Options?)

Initializes a legacy HTTP CONNECT configuration for a proxy server accessible using HTTP/1.1.

init(socksv5Proxy: NWEndpoint)

Initializes a SOCKSv5 proxy configuration.

