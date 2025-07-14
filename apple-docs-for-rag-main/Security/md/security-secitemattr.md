

- Security
-  SecItemAttr 

Enumeration

# SecItemAttr

Specifies a keychain item’s attributes.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecItemAttr
```

## Overview

Not all of these attributes are used for all types of items. Which set of attributes exist for each type of item is documented in the “Data Storage Library Services” chapter of *Common Security: CDSA and CSSM, version 2 (with corrigenda)* from The Open Group (http://www.opengroup.org/security/cdsa.htm) for standard items and in the DL section of the *Security Release Notes* for Apple-defined item types (if any).

To obtain information about a certificate, use the CDSA Certificate Library (CL) API. To obtain information about a key, use the `SecKeyGetCSSMKey` function and the CDSA Cryptographic Service Provider (CSP) API.

For attributes for keys, see Keychain Item Attribute Constants For Keys.

## Topics

### Constants

case creationDateItemAttr

Identifies the creation date attribute.

case modDateItemAttr

Identifies the modification date attribute.

case descriptionItemAttr

Identifies the description attribute.

case commentItemAttr

Identifies the comment attribute.

case creatorItemAttr

Identifies the creator attribute.

case typeItemAttr

Identifies the type attribute.

case scriptCodeItemAttr

Identifies the script code attribute.

case labelItemAttr

Identifies the label attribute.

case invisibleItemAttr

Identifies the invisible attribute.

case negativeItemAttr

Identifies the negative attribute.

case customIconItemAttr

Identifies the custom icon attribute.

case accountItemAttr

Identifies the account attribute.

case serviceItemAttr

Identifies the service attribute.

case genericItemAttr

Identifies the generic attribute.

case securityDomainItemAttr

Identifies the security domain attribute.

case serverItemAttr

Identifies the server attribute.

case authenticationTypeItemAttr

Identifies the authentication type attribute.

case portItemAttr

Identifies the port attribute.

case pathItemAttr

Identifies the path attribute.

case volumeItemAttr

Identifies the volume attribute.

case addressItemAttr

Identifies the address attribute.

case signatureItemAttr

Identifies the server signature attribute.

case protocolItemAttr

Identifies the protocol attribute.

case certificateType

Indicates a `CSSM_CERT_TYPE` type.

case certificateEncoding

Indicates a `CSSM_CERT_ENCODING` type.

case crlType

Indicates a `CSSM_CRL_TYPE` type.

case crlEncoding

Indicates a `CSSM_CRL_ENCODING` type.

case alias

Indicates an alias.

### Initializers

init?(rawValue: FourCharCode)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

