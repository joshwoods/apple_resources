

- Network Extension
-  NWHostEndpoint Deprecated

Class

# NWHostEndpoint

A network endpoint specified by DNS name (or IP address) and port.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class NWHostEndpoint
```

Deprecated

Use the nw_endpoint_t type from the Network framework instead.

## Topics

### Initializing host endpoints

convenience init(hostname: String, port: String)

Create a host endpoint with a hostname and port.

### Getting endpoint properties

var hostname: String

The endpoint’s hostname.

var port: String

The endpoint’s port, represented as a string.

## Relationships

### Inherits From

- NWEndpoint

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

### Endpoints

class NWBonjourServiceEndpoint

A network endpoint specified as a Bonjour service name, type, and domain.

Deprecated

class NWEndpoint

An abstract base class, shared by NWHostEndpoint or NWBonjourServiceEndpoint, that represents the source or destination of a network connection.

Deprecated

