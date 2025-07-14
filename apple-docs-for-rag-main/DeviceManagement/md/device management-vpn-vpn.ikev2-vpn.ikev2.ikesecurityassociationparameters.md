

- Device Management
- VPN
- VPN.IKEv2
-  VPN.IKEv2.IKESecurityAssociationParameters 

Device Management Profile

# VPN.IKEv2.IKESecurityAssociationParameters

The dictionary that contains security association parameters.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.IKEv2.IKESecurityAssociationParameters
```

## Properties

`DiffieHellmanGroup`

`integer`

The Diffie-Hellman group.

For `AlwaysOn` VPN in iOS 14.2 and later, the minimum allowed value is `14`.

In watchOS and tvOS, the minimum allowed value is `14`.

Default: `14`

Possible Values: `1, 2, 5, 14, 15, 16, 17, 18, 19, 20, 21, 31, 32`

`EncryptionAlgorithm`

`string`

The encryption algorithm.

In watchOS and tvOS, the default value is `AES-256-GCM`.

Default: `AES-256`

Possible Values: `DES, 3DES, AES-128, AES-256, AES-128-GCM, AES-256-GCM, ChaCha20Poly1305`

`IntegrityAlgorithm`

`string`

The integrity algorithm.

In watchOS and tvOS, the minimum allowed value is `SHA-2`.

Default: `SHA2-256`

Possible Values: `SHA1-96, SHA1-160, SHA2-256, SHA2-384, SHA2-512`

`LifeTimeInMinutes`

`integer`

The SA lifetime (rekey interval) in minutes.

Default: `1440`

Minimum: `10`

Maximum: `1440`

## See Also

### Objects

object VPN.IKEv2.ChildSecurityAssociationParameters

The dictionary that contains child security association parameters.

