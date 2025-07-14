

- Network
- NWParameters
-  NWParameters.PrivacyContext 

Class

# NWParameters.PrivacyContext

An object that defines the privacy requirements for a set of connections.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class PrivacyContext
```

## Topics

### Configuring Custom Privacy Settings

init(description: String)

Initializes a privacy context with a description string.

static let `default`: NWParameters.PrivacyContext

The privacy context that applies to all connections that do not use a custom context.

func disableLogging()

Disables system logging of connection activity.

func flushCache()

Flushes all cached data, such as TLS session state, created by connections associated with the privacy context.

### Requiring Encrypted DNS

func requireEncryptedNameResolution(Bool, fallbackResolver: NWParameters.PrivacyContext.ResolverConfiguration?)

Requires that any DNS name resolution for connections associated with this context use encrypted transports, such as TLS or HTTPS.

enum ResolverConfiguration

A DNS server configuration that uses TLS or HTTPS.

### Configuring Proxies

var proxyConfigurations: [ProxyConfiguration]

Applies proxy configurations for all connections associated with this context.

struct ProxyConfiguration

A proxy configuration for Relays, Oblivious HTTP, HTTP CONNECT, or SOCKSv5.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Configuring Privacy Settings

func setPrivacyContext(NWParameters.PrivacyContext)

Associates a privacy context with any connections or listeners that use the parameters.

