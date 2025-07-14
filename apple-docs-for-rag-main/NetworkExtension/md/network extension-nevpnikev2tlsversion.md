

- Network Extension
-  NEVPNIKEv2TLSVersion 

Enumeration

# NEVPNIKEv2TLSVersion

An enumeration of TLS Versions for use in EAP-TLS.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 17.0+visionOS 1.0+

``` source
enum NEVPNIKEv2TLSVersion
```

## Topics

### TLS versions

case versionDefault

A value to use the default TLS configuration.

case version1_0

A value to use TLS version 1.0.

case version1_1

A value to use TLS version 1.1.

case version1_2

A value to use TLS version 1.2.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing TLS version properties

var minimumTLSVersion: NEVPNIKEv2TLSVersion

The minimum TLS version to allow for EAP-TLS authentication.

var maximumTLSVersion: NEVPNIKEv2TLSVersion

The minimum TLS version to allow for EAP-TLS authentication.

