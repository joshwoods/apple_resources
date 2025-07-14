

- Security
-  SecExternalFormat 

Enumeration

# SecExternalFormat

The external format of a keychain item.

macOS 10.0+

``` source
enum SecExternalFormat
```

## Topics

### Constants

case formatUnknown

case formatOpenSSL

Format for asymmetric (public/private) keys. OpenSSL is an open source toolkit for Secure Sockets Layer (SSL) and Transport Layer Security (TLS). Also known as X.509 for public keys.

case formatSSH

OpenSSH 1 format for asymmetric (public/private) keys. OpenSSH is an OpenBSD implementation of the Secure Shell (SSH) protocol.

case formatBSAFE

Format for asymmetric keys. BSAFE is a standard from RSA Security for encryption, digital signatures, and privacy.

case formatSSHv2

OpenSSH 2 format for public keys. OpenSSH version 2 private keys are in format `kSecFormatOpenSSL` or `kSecFormatWrappedOpenSSL`. OpenSSH is an OpenBSD implementation of the Secure Shell (SSH) protocol.

case formatRawKey

Format for symmetric keys. Raw, unformatted key bits. This is the default for symmetric keys.

case formatWrappedPKCS8

Format for wrapped symmetric and private keys. PKCS8 is the Private-Key Information Syntax Standard from RSA Security.

case formatWrappedOpenSSL

Format for wrapped symmetric and private keys. OpenSSL is an open-source toolkit for Secure Sockets Layer (SSL) and Transport Layer Security (TLS).

case formatWrappedSSH

OpenSSH 1 format for wrapped symmetric and private keys. OpenSSH is an OpenBSD implementation of the Secure Shell (SSH) protocol.

case formatWrappedLSH

Not supported.

case formatX509Cert

Format for certificates. DER (distinguished encoding rules) encoded. X.509 is a standard for digital certificates from the International Telecommunication Union (ITU). This is the default for certificates.

case formatPEMSequence

Sequence of certificates and keys with PEM armor. PEM armor refers to a way of expressing binary data as an ASCII string so that it can be transferred over text-only channels such as email. This is the default format for multiple items.

case formatPKCS7

Sequence of certificates, no PEM armor. PKCS7 is the Cryptographic Message Syntax Standard from RSA Security, Inc.

case formatPKCS12

Set of certificates and private keys. PKCS12 is the Personal Information Exchange Syntax from RSA Security, Inc.

case formatNetscapeCertSequence

Set of certificates in the Netscape Certificate Sequence format.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

