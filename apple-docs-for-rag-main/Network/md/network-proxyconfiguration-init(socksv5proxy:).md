

- Network
- ProxyConfiguration
-  init(socksv5Proxy:) 

Initializer

# init(socksv5Proxy:)

Initializes a SOCKSv5 proxy configuration.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(socksv5Proxy: NWEndpoint)
```

## Parameters 

`socksv5Proxy`  

A host endpoint identifying the SOCKS proxy server.

## See Also

### Creating Proxy Configurations

init(relayHops: [ProxyConfiguration.RelayHop])

Initializes a proxy configuration with one or two relay hops.

struct RelayHop

A single relay server you can chain together with other servers.

init(httpCONNECTProxy: NWEndpoint, tlsOptions: NWProtocolTLS.Options?)

Initializes a legacy HTTP CONNECT configuration for a proxy server accessible using HTTP/1.1.

