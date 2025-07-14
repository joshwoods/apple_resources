

- Security
-  SSLSetEncryptionCertificate(\_:\_:) Deprecated

Function

# SSLSetEncryptionCertificate(\_:\_:)

Specifies the encryption certificates used for this connection.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.11Deprecated

``` source
func SSLSetEncryptionCertificate(
    _ context: SSLContext,
    _ certRefs: CFArray
) -> OSStatus
```

Deprecated

Using separate RSA certificates for encryption and signing is no longer supported.

## Parameters 

`context`  

An SSL session context reference.

`certRefs`  

A value of type `CFArrayRef` referring to an array of certificate references. The references are type `SecCertificateRef`, except for `certRefs[0]`, which is of type `SecIdentityRef`.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

Use this function in one of the following cases:

- The leaf certificate specified in the SSLSetCertificate(_:_:) function is not capable of encryption.

- The leaf certificate specified in the SSLSetCertificate(_:_:) function contains a key that is too large or strong for legal encryption in this session. In this case, a weaker certificate is specified here and is used for server-initiated key exchange.

The following assumptions are made:

- The `certRefs` parameter’s references remain valid for the lifetime of the connection.

- The specified `certRefs[0]` value is capable of encryption.

This function can be called only when no session is active.

SSL servers that enforce the SSL3 or TLS1 specification to the letter do not accept encryption certificates with key sizes larger than 512 bits for exportable ciphers (that is, for SSL sessions with 40-bit session keys). Therefore, if you wish to support exportable ciphers and your certificate has a key larger than 512 bits, you must specify a separate encryption certificate.

