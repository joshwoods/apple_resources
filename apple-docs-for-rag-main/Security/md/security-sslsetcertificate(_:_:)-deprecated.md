

- Security
-  SSLSetCertificate(\_:\_:) Deprecated

Function

# SSLSetCertificate(\_:\_:)

Specifies this connection’s certificate or certificates.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLSetCertificate(
    _ context: SSLContext,
    _ certRefs: CFArray?
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`certRefs`  

The certificates to set. This array contains items of type `SecCertificateRef`, except for `certRefs[0]`, which is of type `SecIdentityRef`.

## Return Value

A result code. See Secure Transport Result Codes.

## Mentioned in 

Using the Secure Socket Layer for Network Communication

## Discussion

Setting the certificate or certificates is mandatory for server connections, but is optional for clients. Specifying a certificate for a client enables SSL client-side authentication. You must place in `certRefs[0]` a `SecIdentityRef` object that identifies the leaf certificate and its corresponding private key. Specifying a root certificate is optional; if it’s not specified, the root certificate that verifies the certificate chain specified here must be present in the system wide set of trusted anchor certificates.

This function must be called before calling SSLHandshake(_:), or immediately after SSLHandshake(_:) has returned `errSSLClientCertRequested` (that is, before the handshake is resumed by calling SSLHandshake(_:) again).

Secure Transport assumes the following:

- The certificate references remain valid for the lifetime of the session.

- The identity specified in `certRefs[0]` is capable of signing.

The required capabilities of the identity specified in `certRefs[0]`—and of the optional certificate specified in the SSLSetEncryptionCertificate(_:_:) function—are highly dependent on the application. For example, to work as a server with Netscape clients, the identity specified here must be capable of both signing and encrypting. Use the SSLCopyDistinguishedNames(_:_:) function to get a list of certificates acceptable to the server.

