

- Network
-  ProxyConfiguration 

Structure

# ProxyConfiguration

A proxy configuration for Relays, Oblivious HTTP, HTTP CONNECT, or SOCKSv5.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ProxyConfiguration
```

## Topics

### Creating Proxy Configurations

init(relayHops: [ProxyConfiguration.RelayHop])

Initializes a proxy configuration with one or two relay hops.

struct RelayHop

A single relay server you can chain together with other servers.

init(httpCONNECTProxy: NWEndpoint, tlsOptions: NWProtocolTLS.Options?)

Initializes a legacy HTTP CONNECT configuration for a proxy server accessible using HTTP/1.1.

init(socksv5Proxy: NWEndpoint)

Initializes a SOCKSv5 proxy configuration.

### Customizing Proxy Behavior

var allowFailover: Bool

A Boolean that indicates whether or not a proxy configuration allows failover to non-proxied connections. Failover isn’t allowed by default.

func applyCredential(username: String, password: String)

Sets a username and password to use as authentication for a proxy configuration.

### Initializers

init(obliviousHTTPRelay: ProxyConfiguration.RelayHop, relayResourcePath: String, gatewayKeyConfig: Data, matchDomains: [String])

### Instance Properties

var excludedDomains: [String]

var matchDomains: [String]

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Configuring Proxies

var proxyConfigurations: [ProxyConfiguration]

Applies proxy configurations for all connections associated with this context.

