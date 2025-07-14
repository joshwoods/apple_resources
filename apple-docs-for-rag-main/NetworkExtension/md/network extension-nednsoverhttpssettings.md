

- Network Extension
-  NEDNSOverHTTPSSettings 

Class

# NEDNSOverHTTPSSettings

The DNS resolver settings for a DNS-over-HTTPS server.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
class NEDNSOverHTTPSSettings
```

## Topics

### Configuring server properties

var serverURL: URL?

The URL of a DNS-over-HTTPS server.

init(servers: [String])

Initialize the `NEDNSSetting` object.

var matchDomains: [String]?

A list of domain strings used to determine which DNS queries will use the DNS resolver settings contained in this object.

### Configuring client properties

var identityReference: Data?

A persistent keychain reference to a keychain item containing the certificate and private key components of the DNS client credential.

## Relationships

### Inherits From

- NEDNSSettings

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

### DNS configuration

class NEDNSSettingsManager

An object you use to create and manage a DNS settings configuration.

class NEDNSOverTLSSettings

The DNS resolver settings for a DNS-over-TLS server.

