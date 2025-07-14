

- Security
- Secure Transport
-  Secure Transport Result Codes 

API Collection

# Secure Transport Result Codes

Recognize result codes specific to the secure transport API.

## Discussion

Use the SecCopyErrorMessageString(_:_:) function to obtain a human readable string corresponding to these status codes.

The functions of the Secure Transport API may also return the general codes listed in Security Framework Result Codes.

Errors in the range of –9819 through –9840 are fatal errors that are detected by the peer.

## Topics

### App Transport Security result codes

var errSSLATSViolation: OSStatus

An App Transport Security violation occurred.

var errSSLATSMinimumVersionViolation: OSStatus

The minimum protocol version isn’t App Transport Security compliant.

var errSSLATSCiphersuiteViolation: OSStatus

The selected ciphersuite isn’t App Transport Security compliant.

var errSSLATSMinimumKeySizeViolation: OSStatus

The peer key size isn’t App Transport Security compliant.

var errSSLATSLeafCertificateHashAlgorithmViolation: OSStatus

The peer leaf certificate hash algorithm isn’t App Transport Security compliant.

var errSSLATSCertificateHashAlgorithmViolation: OSStatus

The peer certificate hash algorithm isn’t App Transport Security compliant.

var errSSLATSCertificateTrustViolation: OSStatus

The peer certificate wasn’t issued by a trusted peer.

### Certificate issue result codes

var errSSLBadCert: OSStatus

Bad certificate format.

var errSSLBadCertificateStatusResponse: OSStatus

Bad OCSP response.

var errSSLCertExpired: OSStatus

The certificate chain had an expired certificate.

var errSSLCertNotYetValid: OSStatus

The certificate chain had a certificatethat is not yet valid.

var errSSLCertificateRequired: OSStatus

Certificate required.

var errSSLClientCertRequested: OSStatus

The server has requested a client certificate.

var errSSLHostNameMismatch: OSStatus

The host name you connected with does not match any of the host names allowed by the certificate.

var errSSLNoRootCert: OSStatus

No root certificate for the certificate chain.

var errSSLPeerBadCert: OSStatus

A bad certificate was encountered.

var errSSLPeerCertExpired: OSStatus

The certificate expired.

var errSSLPeerCertRevoked: OSStatus

The certificate was revoked.

var errSSLPeerCertUnknown: OSStatus

The certificate is unknown.

var errSSLPeerUnsupportedCert: OSStatus

An unsupported certificate format was encountered.

var errSSLUnknownRootCert: OSStatus

Certificate chain is valid, but root is nottrusted.

var errSSLXCertChainInvalid: OSStatus

Invalid certificate chain.

var errSSLPeerUnknownCA: OSStatus

An unknown certificate authority was encountered.

### Connection status result codes

var errSSLClientHelloReceived: OSStatus

A non-fatal result for providing a server name indication.

var errSSLClosedAbort: OSStatus

The connection closed due to an error.

var errSSLClosedGraceful: OSStatus

The connection closed gracefully.

var errSSLClosedNoNotify: OSStatus

The server closed the session with no notification.

var errSSLConnectionRefused: OSStatus

The peer dropped the connection before responding.

var errSSLPeerAuthCompleted: OSStatus

A non-fatal result indicating the peer certificate is valid, or was ignored if verification is disabled.

var errSSLWouldBlock: OSStatus

Function is blocked; waiting for I/O. This is not fatal.

### Cryptography result codes

var errSSLCrypto: OSStatus

An underlying cryptographic error was encountered.

var errSSLDecryptionFail: OSStatus

Decryption failed.

var errSSLPeerDecryptError: OSStatus

A decryption error occurred.

var errSSLPeerDecryptionFail: OSStatus

Decryption failed.

var errSSLWeakPeerEphemeralDHKey: OSStatus

Indicates a weak ephemeral dh key.

### Other result codes

var errSSLBadCipherSuite: OSStatus

A bad SSL cipher suite was encountered.

var errSSLBadConfiguration: OSStatus

A configuration error occurred.

var errSSLBadRecordMac: OSStatus

A record with a bad message authentication code (MAC) was encountered.

var errSSLBufferOverflow: OSStatus

An insufficient buffer was provided.

var errSSLConfigurationFailed: OSStatus

TLS configuration failed.

var errSSLDecodeError: OSStatus

Decode failed.

var errSSLDecompressFail: OSStatus

Decompression failed.

var errSSLFatalAlert: OSStatus

A fatal alert was encountered.

var errSSLHandshakeFail: OSStatus

Handshake failed.

var errSSLIllegalParam: OSStatus

An illegal parameter was encountered.

var errSSLInappropriateFallback: OSStatus

Inappropriate fallback.

var errSSLInternal: OSStatus

Internal error.

var errSSLMissingExtension: OSStatus

Missing extension.

var errSSLModuleAttach: OSStatus

Module attach failure.

var errSSLNegotiation: OSStatus

The cipher suite negotiation failed.

var errSSLNetworkTimeout: OSStatus

Network timeout triggered.

var errSSLPeerAccessDenied: OSStatus

Access was denied.

var errSSLPeerBadRecordMac: OSStatus

A record with a bad message authentication code (MAC) was encountered.

var errSSLPeerDecodeError: OSStatus

A decoding error occurred.

var errSSLPeerDecompressFail: OSStatus

Decompression failed.

var errSSLPeerExportRestriction: OSStatus

An export restriction occurred.

var errSSLPeerHandshakeFail: OSStatus

The handshake failed.

var errSSLPeerInsufficientSecurity: OSStatus

There is insufficient security for this operation.

var errSSLPeerInternalError: OSStatus

An internal error occurred.

var errSSLPeerNoRenegotiation: OSStatus

No renegotiation is allowed.

var errSSLPeerProtocolVersion: OSStatus

A bad protocol version was encountered.

var errSSLPeerRecordOverflow: OSStatus

A record overflow occurred.

var errSSLPeerUnexpectedMsg: OSStatus

An unexpected message was received.

var errSSLPeerUserCancelled: OSStatus

The user canceled the operation.

var errSSLProtocol: OSStatus

SSL protocol error.

var errSSLRecordOverflow: OSStatus

A record overflow occurred.

var errSSLSessionNotFound: OSStatus

An attempt to restore an unknown session failed.

var errSSLTransportReset: OSStatus

Transport (socket) shutdown, for example, TCP RST or FIN.

var errSSLUnexpectedMessage: OSStatus

Peer rejected unexpected message.

var errSSLUnexpectedRecord: OSStatus

var errSSLUnknownPSKIdentity: OSStatus

Unknown PSK identity.

var errSSLUnrecognizedName: OSStatus

Unknown or unrecognized name.

var errSSLUnsupportedExtension: OSStatus

Unsupported TLS extension.

