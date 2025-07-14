

- Network Extension
-  NEHotspotEAPSettings 

Class

# NEHotspotEAPSettings

Extensible Authentication Protocol settings for configuring WPA and WPA2 enterprise Wi-Fi networks.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class NEHotspotEAPSettings
```

## Topics

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

enum TLSVersion

The EAPTLS Version identifiers that may be specified by preferredTLSVersion.

var outerIdentity: String

The identity string to be used in the EAP-Identity/Response packet during outer EAP authentication.

var ttlsInnerAuthenticationType: NEHotspotEAPSettings.TTLSInnerAuthenticationType

The inner-layer authentication protocol used by a TTLS module.

enum TTLSInnerAuthenticationType

The TTLS Inner Authentication Types that may be specified by NEHotspotEAPSettings.TTLSInnerAuthenticationType.

### Setting Keychain-based EAP Properties

func setIdentity(SecIdentity) -> Bool

Sets the client identity for EAP authentication.

func setTrustedServerCertificates([Any]) -> Bool

Sets trusted EAP server certificates for an enterprise Wi-Fi or Hotspot 2.0 network.

## Relationships

### Inherits From

- NSObject

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

### Wi-Fi network configuration

class NEHotspotConfigurationManager

A manager that applies and removes hotspot configurations of Wi-Fi networks.

class NEHotspotConfiguration

Configuration settings for a Wi-Fi network.

class NEHotspotHS20Settings

Settings for configuring Hotspot 2.0 Wi-Fi networks.

