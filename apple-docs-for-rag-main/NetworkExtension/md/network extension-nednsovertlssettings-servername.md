

- Network Extension
- NEDNSOverTLSSettings
-  serverName 

Instance Property

# serverName

The TLS name of a DNS-over-TLS server.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
var serverName: String? { get set }
```

## Discussion

The server will be accessed over TCP port 853, as defined in RFC 7858. The server name is used for TLS validation.

## See Also

### Configuring server properties

init(servers: [String])

Initialize the `NEDNSSetting` object.

var matchDomains: [String]?

A list of domain strings used to determine which DNS queries will use the DNS resolver settings contained in this object.

