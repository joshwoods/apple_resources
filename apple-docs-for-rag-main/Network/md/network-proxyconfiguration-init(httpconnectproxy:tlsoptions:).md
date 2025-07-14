

- Network
- ProxyConfiguration
-  init(httpCONNECTProxy:tlsOptions:) 

Initializer

# init(httpCONNECTProxy:tlsOptions:)

Initializes a legacy HTTP CONNECT configuration for a proxy server accessible using HTTP/1.1.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    httpCONNECTProxy: NWEndpoint,
    tlsOptions: NWProtocolTLS.Options? = nil
)
```

## Parameters 

`httpCONNECTProxy`  

A host endpoint identifying the proxy server accessible using HTTP/1.1.

`tlsOptions`  

Optional TLS options to use for a TLS handshake to the relay. If no TLS options are provided, the proxy will be accessed using cleartext HTTP.

## Discussion

These HTTP CONNECT proxies only handle TCP connections. To support UDP proxying, use init(relayHops:).

## See Also

### Creating Proxy Configurations

init(relayHops: [ProxyConfiguration.RelayHop])

Initializes a proxy configuration with one or two relay hops.

struct RelayHop

A single relay server you can chain together with other servers.

init(socksv5Proxy: NWEndpoint)

Initializes a SOCKSv5 proxy configuration.

