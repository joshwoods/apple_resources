

- Network
- NWParameters
- NWParameters.PrivacyContext
- NWParameters.PrivacyContext.ResolverConfiguration
-  NWParameters.PrivacyContext.ResolverConfiguration.tls(\_:serverAddresses:) 

Case

# NWParameters.PrivacyContext.ResolverConfiguration.tls(\_:serverAddresses:)

A DNS-over-TLS resolver configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case tls(
    NWEndpoint,
    serverAddresses: [NWEndpoint]
)
```

## Discussion

The hostname of the provided endpoint will be used to validate the TLS certificate of the server. See RFC 7858 for more details. The associated server addresses you provide are hints for which well-known DNS server addresses to use.

## See Also

### Resolver Types

case https(URL, serverAddresses: [NWEndpoint])

A DNS-over-HTTPS resolver configuration.

