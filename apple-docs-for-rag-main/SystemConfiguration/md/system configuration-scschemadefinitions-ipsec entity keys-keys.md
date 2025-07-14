

- System Configuration
- SCSchemaDefinitions
-  IPSec Entity Keys 

API Collection

# IPSec Entity Keys

Keys that correspond to values in the `kSCEntNetIPSec` dictionary.

## Topics

### Constants

let kSCPropNetIPSecLocalIdentifier: CFString

The IPSec key `LocalIdentifier`, whose value is of type `CFString`.

let kSCPropNetIPSecLocalIdentifierType: CFString

The IPSec key `LocalIdentifierType`, whose value is of type `CFString`.

let kSCPropNetIPSecAuthenticationMethod: CFString

The IPSec key `AuthenticationMethod`, whose value is of type `CFString`.

let kSCPropNetIPSecSharedSecret: CFString

The IPSec key `SharedSecret`, whose value is of type `CFString`.

let kSCPropNetIPSecSharedSecretEncryption: CFString

The IPSec key `SharedSecretEncryption`, whose value is of type `CFString`.

let kSCPropNetIPSecLocalCertificate: CFString

The IPSec key `LocalCertificate`, whose value is of type `CFData`.

let kSCPropNetIPSecConnectTime: CFString

The IPSec key ConnectTime.

let kSCPropNetIPSecRemoteAddress: CFString

The IPSec key RemoteAddress.

let kSCPropNetIPSecStatus: CFString

The IPSec key Status.

let kSCPropNetIPSecXAuthEnabled: CFString

The IPSec key XAuthEnabled.

let kSCPropNetIPSecXAuthName: CFString

The IPSec key XAuthName.

let kSCPropNetIPSecXAuthPassword: CFString

The IPSec key XAuthPassword.

let kSCPropNetIPSecXAuthPasswordEncryption: CFString

The IPSec key XAuthPasswordEncryption.

### Authentication Method Values

let kSCValNetIPSecAuthenticationMethodSharedSecret: CFString

The constant value SharedSecret.

let kSCValNetIPSecAuthenticationMethodCertificate: CFString

The constant value Certificate.

let kSCValNetIPSecAuthenticationMethodHybrid: CFString

The constant value Hybrid.

### Local Identifier Type Values

let kSCValNetIPSecLocalIdentifierTypeKeyID: CFString

The constant value KeyID.

### IPSec Shared Secret Encryption Values

let kSCValNetIPSecSharedSecretEncryptionKeychain: CFString

The constant value Keychain.

### XAuth Password Encryption Values

let kSCValNetIPSecXAuthPasswordEncryptionKeychain: CFString

The constant value Keychain.

let kSCValNetIPSecXAuthPasswordEncryptionPrompt: CFString

The constant value Prompt.

## See Also

### Constants

Generic Keys

General-purpose keys that apply to multiple dictionaries in the persistent store.

Preference Keys

Keys that correspond to preferences in the persistent store.

Component Keys

Keys that correspond to components in the persistent store.

Network Dictionary Keys

Keys that correspond to values in the `kSCCompNetwork` dictionary.

Interface Dictionary Keys

Keys that correspond to values in the `kSCCompInterface` dictionary.

Hostnames Dictionary Keys

Keys that correspond to values in the `kSCCompHostnames` dictionary.

Network Entity Keys

Keys that correspond to network entity dictionaries in the persistent store.

DNS Entity Keys

Keys that correspond to values in the `kSCEntNetDNS` dictionary.

Ethernet Entity Keys

Keys that correspond to values in the `kSCEntNetEthernet` dictionary.

Interface Entity Keys

Keys that correspond to values in the `kSCEntNetInterface` dictionary.

IPv4 Entity Keys

Keys that correspond to values in the `kSCEntNetIPv4` dictionary.

IPv6 Entity Keys

Keys that correspond to values in the `kSCEntNetIPv6` dictionary.

6to4 Entity Keys

Keys that correspond to values in the `kSCEntNet6to4` dictionary.

Link Entity Keys

Keys that correspond to values in the `kSCEntNetLink` dictionary.

Modem Entity Keys

Keys that correspond to values in the `kSCEntNetModem` dictionary.

