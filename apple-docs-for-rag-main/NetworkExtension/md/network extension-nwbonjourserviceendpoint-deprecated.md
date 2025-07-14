

- Network Extension
-  NWBonjourServiceEndpoint Deprecated

Class

# NWBonjourServiceEndpoint

A network endpoint specified as a Bonjour service name, type, and domain.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class NWBonjourServiceEndpoint
```

Deprecated

Use the nw_endpoint_t type from the Network framework instead.

## Overview

For example, the Bonjour service `MyMusicStudio._music._tcp.local.` has the name `"MyMusicStudio"`, the type `"_music._tcp"`, and the domain `"local"`.

## Topics

### Initializing Bonjour service endpoints

convenience init(name: String, type: String, domain: String)

Create an endpoint with a Bonjour service name, type, and domain. All fields must be specified.

### Getting endpoint properties

var name: String

The endpoint’s Bonjour service name.

var type: String

The endpoint’s Bonjour service type.

var domain: String

The endpoint’s Bonjour service domain, such as `"local"`.

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

class NWHostEndpoint

A network endpoint specified by DNS name (or IP address) and port.

Deprecated

class NWEndpoint

An abstract base class, shared by NWHostEndpoint or NWBonjourServiceEndpoint, that represents the source or destination of a network connection.

Deprecated

