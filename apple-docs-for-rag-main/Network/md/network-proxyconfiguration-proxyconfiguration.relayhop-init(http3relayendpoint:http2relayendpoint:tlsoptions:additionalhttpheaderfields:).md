

- Network
- ProxyConfiguration
- ProxyConfiguration.RelayHop
-  init(http3RelayEndpoint:http2RelayEndpoint:tlsOptions:additionalHTTPHeaderFields:) 

Initializer

# init(http3RelayEndpoint:http2RelayEndpoint:tlsOptions:additionalHTTPHeaderFields:)

Creates a configuration for a secure relay accessible using HTTP/3, with an optional HTTP/2 fallback.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    http3RelayEndpoint: NWEndpoint,
    http2RelayEndpoint: NWEndpoint? = nil,
    tlsOptions: NWProtocolTLS.Options = .init(),
    additionalHTTPHeaderFields: [String : String] = [:]
)
```

## Parameters 

`http3RelayEndpoint`  

A URL or host endpoint identifying the relay server accessible using HTTP/3.

`http2RelayEndpoint`  

An optional URL or host endpoint identifying the relay server accessible using HTTP/2. This can be the same endpoint as `http3RelayEndpoint`.

`tlsOptions`  

The TLS options to use for the TLS handshake to the relay.

`additionalHTTPHeaderFields`  

A dictionary of additional HTTP headers to send as part of `CONNECT` requests to the relay.

## See Also

### Creating Relay Hops

init(http2RelayEndpoint: NWEndpoint, tlsOptions: NWProtocolTLS.Options, additionalHTTPHeaderFields: [String : String])

Creates a configuration for a secure relay accessible only using HTTP/2.

