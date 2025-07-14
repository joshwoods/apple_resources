

- Network
- NWParameters
- NWParameters.PrivacyContext
- NWParameters.PrivacyContext.ResolverConfiguration
-  NWParameters.PrivacyContext.ResolverConfiguration.https(\_:serverAddresses:) 

Case

# NWParameters.PrivacyContext.ResolverConfiguration.https(\_:serverAddresses:)

A DNS-over-HTTPS resolver configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case https(
    URL,
    serverAddresses: [NWEndpoint]
)
```

## Discussion

The URL describes the location of the DNS server, such as “https://dnsserver.example.net/dns-query”. See RFC 8484 for more details. The associated server addresses you provide are hints for which well-known DNS server addresses to use.

## See Also

### Resolver Types

case tls(NWEndpoint, serverAddresses: [NWEndpoint])

A DNS-over-TLS resolver configuration.

