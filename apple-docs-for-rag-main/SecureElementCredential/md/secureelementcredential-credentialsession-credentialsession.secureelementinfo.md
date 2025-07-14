

- SecureElementCredential
- CredentialSession
-  CredentialSession.SecureElementInfo 

Structure

# CredentialSession.SecureElementInfo

A type that provides information about the Secure Element hardware.

iOS 18.4+iPadOS 18.4+

``` source
struct SecureElementInfo
```

## Topics

### Getting hardware information

let hardwareReleaseVersionInfo: String

A string that encodes the hardware and software release versions of the Secure Element.

let secureElementPlatformSigningCertificate: Data

A certificate you use to authenticate against the Certification Authority of the Secure Element hardware.

### Encoding and decoding

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

## Relationships

### Conforms To

- Decodable
- Encodable

## See Also

### Accessing hardware information

var secureElementInfo: CredentialSession.SecureElementInfo

A property that provides information about the Secure Element hardware.

