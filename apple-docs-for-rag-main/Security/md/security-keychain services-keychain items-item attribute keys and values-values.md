

- Security
- Keychain services
- Keychain items
-  Item attribute keys and values 

API Collection

# Item attribute keys and values

Specify the attributes of keychain items.

## Overview

In addition to the data that you want to store, keychain items also have attributes that allow you to find them later and that allow you to control how the data is used or shared.

You specify attributes as the keys and values of a dictionary. The available attribute keys are listed below. Typically, the corresponding value is a string, a number, or some other basic type, as given in each key description. In a few cases, the value comes instead from a list of a known constants. These predefined attribute values are also listed below, grouped according to the key that they serve.

Note

Not all attributes apply to every item class. You can find the list of attributes applicable to a given class in the relevant item class value definition, namely in kSecClassGenericPassword, kSecClassInternetPassword, kSecClassCertificate, kSecClassIdentity, or kSecClassKey.

## Topics

### General Item Attribute Keys

let kSecAttrAccess: CFString

A key with a value that indicates access control list settings for the item.

let kSecAttrAccessControl: CFString

A key with a value that’s an access control instance indicating access control settings for the item.

let kSecAttrAccessible: CFString

A key with a value that indicates when the keychain item is accessible.

let kSecAttrAccessGroup: CFString

A key with a value that’s a string indicating the access group the item is in.

let kSecAttrSynchronizable: CFString

A key with a value that’s a string indicating whether the item synchronizes through iCloud.

let kSecAttrCreationDate: CFString

A key with a value that indicates the item’s creation date.

let kSecAttrModificationDate: CFString

A key with a value that indicates the item’s most recent modification date.

let kSecAttrDescription: CFString

A key with a value that’s a string indicating the item’s description.

let kSecAttrComment: CFString

A key with a value that’s a string indicating a comment associated with the item.

let kSecAttrCreator: CFString

A key with a value that indicates the item’s creator.

let kSecAttrType: CFString

A key with a value that indicates the item’s type.

let kSecAttrLabel: CFString

A key with a value that’s a string indicating the item’s label.

let kSecAttrIsInvisible: CFString

A key with a value that’s a Boolean indicating the item’s visibility.

let kSecAttrIsNegative: CFString

A key with a value that’s a Boolean indicating whether the item has a valid password.

let kSecAttrSyncViewHint: CFString

A key with a value that’s a string that provides a sync view hint.

let kSecAttrPersistantReference: CFString

let kSecAttrPersistentReference: CFString

let kSecUseUserIndependentKeychain: CFString

A key with a value that indicates whether to store the data in a keychain available to anyone who uses the device.

### Password Attribute Keys

let kSecAttrAccount: CFString

A key whose value is a string indicating the item’s account name.

let kSecAttrService: CFString

A key whose value is a string indicating the item’s service.

let kSecAttrGeneric: CFString

A key whose value indicates the item’s user-defined attributes.

let kSecAttrSecurityDomain: CFString

A key whose value is a string indicating the item’s security domain.

let kSecAttrServer: CFString

A key whose value is a string indicating the item’s server.

let kSecAttrProtocol: CFString

A key whose value indicates the item’s protocol.

let kSecAttrAuthenticationType: CFString

A key whose value indicates the item’s authentication scheme.

let kSecAttrPort: CFString

A key whose value indicates the item’s port.

let kSecAttrPath: CFString

A key whose value is a string indicating the item’s path attribute.

### Certificate Attribute Keys

let kSecAttrSubject: CFString

A key whose value indicates the item’s subject name.

let kSecAttrIssuer: CFString

A key whose value indicates the item’s issuer.

let kSecAttrSerialNumber: CFString

A key whose value indicates the item’s serial number.

let kSecAttrSubjectKeyID: CFString

A key whose value indicates the item’s subject key ID.

let kSecAttrPublicKeyHash: CFString

A key whose value indicates the item’s public key hash.

let kSecAttrCertificateType: CFString

A key whose value indicates the item’s certificate type.

let kSecAttrCertificateEncoding: CFString

A key whose value indicates the item’s certificate encoding.

### Cryptographic Key Attribute Keys

let kSecAttrKeyClass: CFString

A key whose value indicates the item’s cryptographic key class.

let kSecAttrApplicationLabel: CFString

A key whose value indicates the item’s application label.

let kSecAttrApplicationTag: CFString

A key whose value indicates the item’s private tag.

let kSecAttrKeyType: CFString

A key whose value indicates the item’s algorithm.

let kSecAttrPRF: CFString

A key whose value indicates the item’s pseudorandom function.

let kSecAttrSalt: CFString

A key whose value indicates the salt to use for this item.

let kSecAttrRounds: CFString

A key whose value indicates the number of rounds to run the pseudorandom function.

let kSecAttrKeySizeInBits: CFString

A key whose value indicates the number of bits in a cryptographic key.

let kSecAttrEffectiveKeySize: CFString

A key whose value indicates the effective number of bits in a cryptographic key.

let kSecAttrTokenID: CFString

A key whose value indicates that a cryptographic key is in an external store.

### Cryptographic Key Usage Attribute Keys

let kSecAttrIsPermanent: CFString

A key whose value indicates the item’s permanence.

let kSecAttrIsSensitive: CFString

A key whose value indicates the item’s sensitivity.

let kSecAttrIsExtractable: CFString

A key whose value indicates the item’s extractability.

let kSecAttrCanEncrypt: CFString

A key whose value is a Boolean that indicates whether the cryptographic key can be used for encryption.

let kSecAttrCanDecrypt: CFString

A key whose value is a Boolean that indicates whether the cryptographic key can be used for decryption.

let kSecAttrCanDerive: CFString

A key whose value is a Boolean that indicates whether the cryptographic key can be used for derivation.

let kSecAttrCanSign: CFString

A key whose value is a Boolean that indicates whether the cryptographic key can be used for digital signing.

let kSecAttrCanVerify: CFString

A key whose value is a Boolean that indicates whether the cryptographic key can be used for signature verification.

let kSecAttrCanWrap: CFString

A key whose value is a Boolean that indicates whether the cryptographic key can be used for wrapping.

let kSecAttrCanUnwrap: CFString

A key whose value is a Boolean that indicates whether the cryptographic key can be used for unwrapping.

### Protocol Values

Values you use with the kSecAttrProtocol attribute key.

let kSecAttrProtocolFTP: CFString

FTP protocol.

let kSecAttrProtocolFTPAccount: CFString

A client side FTP account.

let kSecAttrProtocolHTTP: CFString

HTTP protocol.

let kSecAttrProtocolIRC: CFString

IRC protocol.

let kSecAttrProtocolNNTP: CFString

NNTP protocol.

let kSecAttrProtocolPOP3: CFString

POP3 protocol.

let kSecAttrProtocolSMTP: CFString

SMTP protocol.

let kSecAttrProtocolSOCKS: CFString

SOCKS protocol.

let kSecAttrProtocolIMAP: CFString

IMAP protocol.

let kSecAttrProtocolLDAP: CFString

LDAP protocol.

let kSecAttrProtocolAppleTalk: CFString

AFP over AppleTalk.

let kSecAttrProtocolAFP: CFString

AFP over TCP.

let kSecAttrProtocolTelnet: CFString

Telnet protocol.

let kSecAttrProtocolSSH: CFString

SSH protocol.

let kSecAttrProtocolFTPS: CFString

FTP over TLS/SSL.

let kSecAttrProtocolHTTPS: CFString

HTTP over TLS/SSL.

let kSecAttrProtocolHTTPProxy: CFString

HTTP proxy.

let kSecAttrProtocolHTTPSProxy: CFString

HTTPS proxy.

let kSecAttrProtocolFTPProxy: CFString

FTP proxy.

let kSecAttrProtocolSMB: CFString

SMB protocol.

let kSecAttrProtocolRTSP: CFString

RTSP protocol.

let kSecAttrProtocolRTSPProxy: CFString

RTSP proxy.

let kSecAttrProtocolDAAP: CFString

DAAP protocol.

let kSecAttrProtocolEPPC: CFString

Remote Apple Events.

let kSecAttrProtocolIPP: CFString

IPP protocol.

let kSecAttrProtocolNNTPS: CFString

NNTP over TLS/SSL.

let kSecAttrProtocolLDAPS: CFString

LDAP over TLS/SSL.

let kSecAttrProtocolTelnetS: CFString

Telnet over TLS/SSL.

let kSecAttrProtocolIMAPS: CFString

IMAP over TLS/SSL.

let kSecAttrProtocolIRCS: CFString

IRC over TLS/SSL.

let kSecAttrProtocolPOP3S: CFString

POP3 over TLS/SSL.

### Authentication Type Values

Values you use with the kSecAttrAuthenticationType attribute key.

let kSecAttrAuthenticationTypeNTLM: CFString

Windows NT LAN Manager authentication.

let kSecAttrAuthenticationTypeMSN: CFString

Microsoft Network default authentication.

let kSecAttrAuthenticationTypeDPA: CFString

Distributed Password authentication.

let kSecAttrAuthenticationTypeRPA: CFString

Remote Password authentication.

let kSecAttrAuthenticationTypeHTTPBasic: CFString

HTTP Basic authentication.

let kSecAttrAuthenticationTypeHTTPDigest: CFString

HTTP Digest Access authentication.

let kSecAttrAuthenticationTypeHTMLForm: CFString

HTML form based authentication.

let kSecAttrAuthenticationTypeDefault: CFString

The default authentication type.

### Key Class Values

Values you use with the kSecAttrKeyClass attribute key.

let kSecAttrKeyClassPublic: CFString

A public key of a public-private pair.

let kSecAttrKeyClassPrivate: CFString

A private key of a public-private pair.

let kSecAttrKeyClassSymmetric: CFString

A private key used for symmetric-key encryption and decryption.

### Key Type Values

Values you use with the kSecAttrKeyType attribute key.

let kSecAttrKeyTypeRSA: CFString

RSA algorithm.

let kSecAttrKeyTypeDSA: CFString

DSA algorithm.

let kSecAttrKeyTypeAES: CFString

AES algorithm.

let kSecAttrKeyTypeDES: CFString

DES algorithm.

let kSecAttrKeyType3DES: CFString

3DES algorithm.

let kSecAttrKeyTypeRC4: CFString

RC4 algorithm.

let kSecAttrKeyTypeRC2: CFString

RC2 algorithm.

let kSecAttrKeyTypeCAST: CFString

CAST algorithm.

let kSecAttrKeyTypeECDSA: CFString

Elliptic curve DSA algorithm.

Deprecated

let kSecAttrKeyTypeEC: CFString

Elliptic curve algorithm.

Deprecated

let kSecAttrKeyTypeECSECPrimeRandom: CFString

Elliptic curve algorithm.

### Synchronizability Values

Values you use with the kSecAttrSynchronizable attribute key.

let kSecAttrSynchronizableAny: CFString

Specifies that both synchronizable and non-synchronizable results should be returned from a query.

### Token ID Values

Values you use with the kSecAttrTokenID attribute key.

let kSecAttrTokenIDSecureEnclave: CFString

Specifies an item should be stored in the device’s Secure Enclave.

### Accessibility Values

Values you use with the kSecAttrAccessible attribute key, listed from most to least restrictive.

let kSecAttrAccessibleWhenPasscodeSetThisDeviceOnly: CFString

The data in the keychain can only be accessed when the device is unlocked. Only available if a passcode is set on the device.

let kSecAttrAccessibleWhenUnlockedThisDeviceOnly: CFString

The data in the keychain item can be accessed only while the device is unlocked by the user.

let kSecAttrAccessibleWhenUnlocked: CFString

The data in the keychain item can be accessed only while the device is unlocked by the user.

let kSecAttrAccessibleAfterFirstUnlockThisDeviceOnly: CFString

The data in the keychain item cannot be accessed after a restart until the device has been unlocked once by the user.

let kSecAttrAccessibleAfterFirstUnlock: CFString

The data in the keychain item cannot be accessed after a restart until the device has been unlocked once by the user.

let kSecAttrAccessibleAlwaysThisDeviceOnly: CFString

The data in the keychain item can always be accessed regardless of whether the device is locked.

Deprecated

let kSecAttrAccessibleAlways: CFString

The data in the keychain item can always be accessed regardless of whether the device is locked.

Deprecated

### Pseudorandom Function Values

Values you use with the kSecAttrPRF attribute key to indicate the item’s pseudorandom function.

let kSecAttrPRFHmacAlgSHA1: CFString

Use the SHA1 algorithm.

let kSecAttrPRFHmacAlgSHA224: CFString

Use the SHA224 algorithm.

let kSecAttrPRFHmacAlgSHA256: CFString

Use the SHA256 algorithm.

let kSecAttrPRFHmacAlgSHA384: CFString

Use the SHA384 algorithm.

let kSecAttrPRFHmacAlgSHA512: CFString

Use the SHA512 algorithm.

### Access Group Values

Values you use with the kSecAttrAccessGroup attribute key.

let kSecAttrAccessGroupToken: CFString

The access group containing items provided by external tokens.

