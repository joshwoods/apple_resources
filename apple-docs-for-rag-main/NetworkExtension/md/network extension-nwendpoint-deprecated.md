

- Network Extension
-  NWEndpoint Deprecated

Class

# NWEndpoint

An abstract base class, shared by NWHostEndpoint or NWBonjourServiceEndpoint, that represents the source or destination of a network connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class NWEndpoint
```

Deprecated

Use the nw_endpoint_t type from the Network framework instead.

## Overview

All endpoint objects are static collections of parameters that describe a network resource. They do not directly provide any resolution services, but instead must be used with other classes to be resolved and create connections.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NWBonjourServiceEndpoint
- NWHostEndpoint

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

class NWHostEndpoint

A network endpoint specified by DNS name (or IP address) and port.

Deprecated

class NWBonjourServiceEndpoint

A network endpoint specified as a Bonjour service name, type, and domain.

Deprecated

