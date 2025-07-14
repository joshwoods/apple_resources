

- Network Extension
-  NEDNSSettings 

Class

# NEDNSSettings

The DNS resolver settings of a network tunnel or a system-wide configuration.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEDNSSettings
```

## Topics

### Initializing DNS settings

init(servers: [String])

Initialize the `NEDNSSetting` object.

### Accessing DNS properties

var servers: [String]

The DNS server IP addresses.

var searchDomains: [String]?

A list of domain strings used to fully qualify single-label host names.

var domainName: String?

The primary domain of the tunnel.

var matchDomains: [String]?

A list of domain strings used to determine which DNS queries will use the DNS resolver settings contained in this object.

var matchDomainsNoSearch: Bool

A Boolean that specifies if the domains in the `matchDomains` list should not be appended to the resolver’s list of search domains.

var dnsProtocol: NEDNSProtocol

The DNS protocol used by the server, such as HTTPS or TLS.

enum NEDNSProtocol

## Relationships

### Inherits From

- NSObject

### Inherited By

- NEDNSOverHTTPSSettings
- NEDNSOverTLSSettings

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Related Documentation

class NEDNSOverHTTPSSettings

The DNS resolver settings for a DNS-over-HTTPS server.

class NEDNSOverTLSSettings

The DNS resolver settings for a DNS-over-TLS server.

### Provider

class NEDNSProxyProvider

The principal class for a DNS proxy provider app extension.

