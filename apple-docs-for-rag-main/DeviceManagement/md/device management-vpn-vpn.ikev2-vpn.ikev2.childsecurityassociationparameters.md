

- Device Management
- VPN
- VPN.IKEv2
-  VPN.IKEv2.ChildSecurityAssociationParameters 

Device Management Profile

# VPN.IKEv2.ChildSecurityAssociationParameters

The dictionary that contains child security association parameters.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.IKEv2.ChildSecurityAssociationParameters
```

## Properties

`DiffieHellmanGroup`

`integer`

The Diffie-Hellman group. For AlwaysOn VPN, minimum allowed Diffie Hellman Group is `14` in iOS 14.2 and later.

Default: `14`

Possible Values: `1, 2, 5, 14, 15, 16, 17, 18, 19, 20, 21, 31, 32`

`EncryptionAlgorithm`

`string`

The encryption algorithm.

Default: `AES-256`

Possible Values: `DES, 3DES, AES-128, AES-256, AES-128-GCM, AES-256-GCM, ChaCha20Poly1305`

`IntegrityAlgorithm`

`string`

The integrity algorithm.

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

object VPN.IKEv2.IKESecurityAssociationParameters

The dictionary that contains security association parameters.

