

- Network Extension
- NEDNSOverHTTPSSettings
-  serverURL 

Instance Property

# serverURL

The URL of a DNS-over-HTTPS server.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
var serverURL: URL? { get set }
```

## Discussion

The URL should use the URI template format defined by RFC 8484, for example `https://dnsserver.example.net/dns-query`.

## See Also

### Configuring server properties

init(servers: [String])

Initialize the `NEDNSSetting` object.

var matchDomains: [String]?

A list of domain strings used to determine which DNS queries will use the DNS resolver settings contained in this object.

