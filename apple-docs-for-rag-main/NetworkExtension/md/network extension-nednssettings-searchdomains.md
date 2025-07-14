

- Network Extension
- NEDNSSettings
-  searchDomains 

Instance Property

# searchDomains

A list of domain strings used to fully qualify single-label host names.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var searchDomains: [String]? { get set }
```

## See Also

### Accessing DNS properties

var servers: [String]

The DNS server IP addresses.

var domainName: String?

The primary domain of the tunnel.

var matchDomains: [String]?

A list of domain strings used to determine which DNS queries will use the DNS resolver settings contained in this object.

var matchDomainsNoSearch: Bool

A Boolean that specifies if the domains in the `matchDomains` list should not be appended to the resolver’s list of search domains.

var dnsProtocol: NEDNSProtocol

The DNS protocol used by the server, such as HTTPS or TLS.

enum NEDNSProtocol

