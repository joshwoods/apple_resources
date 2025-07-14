

- Network Extension
- NEHotspotEAPSettings
-  NEHotspotEAPSettings.TLSVersion 

Enumeration

# NEHotspotEAPSettings.TLSVersion

The EAPTLS Version identifiers that may be specified by preferredTLSVersion.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum TLSVersion
```

## Topics

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

### Accessing EAP properties

var isTLSClientCertificateRequired: Bool

A Boolean value indicating whether a network requires two-factor authentication or allows zero-factor authentication.

var trustedServerNames: [String]

An array of server certificate common name strings used to verify a server’s certificate.

var supportedEAPTypes: [NSNumber]

An array of supported EAP types.

enum EAPType

The EAP types that may be specified in supportedEAPTypes.

var username: String

The user name string for EAP authentication, encoded as UTF-8.

var password: String

The password component of the IEEE 802.1X authentication credential.

var preferredTLSVersion: NEHotspotEAPSettings.TLSVersion

The Transport Layer Security (TLS) version to use during a TLS authentication handshake.

var outerIdentity: String

The identity string to be used in the EAP-Identity/Response packet during outer EAP authentication.

var ttlsInnerAuthenticationType: NEHotspotEAPSettings.TTLSInnerAuthenticationType

The inner-layer authentication protocol used by a TTLS module.

enum TTLSInnerAuthenticationType

The TTLS Inner Authentication Types that may be specified by NEHotspotEAPSettings.TTLSInnerAuthenticationType.

