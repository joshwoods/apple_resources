

- Network
- NWParameters
- NWParameters.PrivacyContext
-  NWParameters.PrivacyContext.ResolverConfiguration 

Enumeration

# NWParameters.PrivacyContext.ResolverConfiguration

A DNS server configuration that uses TLS or HTTPS.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum ResolverConfiguration
```

## Topics

### Resolver Types

case https(URL, serverAddresses: [NWEndpoint])

A DNS-over-HTTPS resolver configuration.

case tls(NWEndpoint, serverAddresses: [NWEndpoint])

A DNS-over-TLS resolver configuration.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Requiring Encrypted DNS

func requireEncryptedNameResolution(Bool, fallbackResolver: NWParameters.PrivacyContext.ResolverConfiguration?)

Requires that any DNS name resolution for connections associated with this context use encrypted transports, such as TLS or HTTPS.

