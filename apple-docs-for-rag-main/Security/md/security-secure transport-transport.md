

- Security
-  Secure Transport 

API Collection

# Secure Transport

Secure network communication using standardized transport layer security mechanisms.

## Overview

The `Security.SecureTransport` API gives you access to Apple’s implementation of Secure Sockets Layer version 3.0 (SSLv3), Transport Layer Security (TLS) versions 1.0 through 1.2, and Datagram Transport Layer Security (DTLS) version 1.0.

This API imposes no transport layer dependencies. You can use it with BSD Sockets and other protocols. To use this API, you provide callback functions to perform I/O on the underlying network connections. You are also responsible for setting up raw network connections. You pass in an opaque reference to the underlying (connected) entity at the start of an SSL session in the form of an SSLConnectionRef object.

Important

This API is considered legacy. Use the Network framework instead.

## Topics

### First Steps

Using the Secure Socket Layer for Network Communication

Establish Secure Sockets Layer (SSL) sessions to facilitate secure communication between client and server.

### Session Context

func SSLCreateContext(CFAllocator?, SSLProtocolSide, SSLConnectionType) -> SSLContext?

Allocates and returns a new context.

Deprecated

enum SSLProtocolSide

The flags that indicate whether a context is for the server or client side of a connection.

enum SSLConnectionType

The flags that indicate whether a context is to be used for streaming or datagram-based communication.

class SSLContext

An opaque type that represents an SSL session context object.

func SSLContextGetTypeID() -> CFTypeID

Returns the Core Foundation type ID for context objects.

Deprecated

### Context Options

func SSLSetSessionOption(SSLContext, SSLSessionOption, Bool) -> OSStatus

Specifies options for a specific session.

Deprecated

func SSLGetSessionOption(SSLContext, SSLSessionOption, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates the current setting of Secure Sockets Layer (SSL) session options.

Deprecated

enum SSLSessionOption

The options that can be set for an SSL session.

### Context Callbacks

func SSLSetIOFuncs(SSLContext, SSLReadFunc, SSLWriteFunc) -> OSStatus

Specifies callback functions that perform the network I/O operations.

Deprecated

typealias SSLReadFunc

A pointer to a customized read function that secure transport calls to read data from the connection.

typealias SSLWriteFunc

A pointer to a customized write function that secure transport calls to write data to the connection.

### Session Configuration

func SSLSetSessionConfig(SSLContext, CFString) -> OSStatus

Sets a predefined configuration for the Secure Sockets Layer (SSL) session.

Deprecated

func SSLSetClientSideAuthenticate(SSLContext, SSLAuthenticate) -> OSStatus

Specifies the requirements for client-side authentication.

Deprecated

SSLConfig

Use these constants to configure Transport Layer Security (TLS) sessions.

enum SSLAuthenticate

The flags that represent the requirements for client-side authentication.

### I/O Connections

func SSLSetConnection(SSLContext, SSLConnectionRef?) -> OSStatus

Specifies an I/O connection for a specific session.

Deprecated

func SSLGetConnection(SSLContext, UnsafeMutablePointer&lt;SSLConnectionRef?>) -> OSStatus

Retrieves an I/O connection—such as a socket or endpoint—for a specific session.

Deprecated

typealias SSLConnectionRef

A pointer to an opaque I/O connection object.

### Session State

func SSLHandshake(SSLContext) -> OSStatus

Performs the SSL handshake.

Deprecated

func SSLReHandshake(SSLContext) -> OSStatus

Requests renegotiation of the SSL handshake. Server only.

Deprecated

func SSLClose(SSLContext) -> OSStatus

Terminates the current SSL session.

Deprecated

func SSLSetPeerID(SSLContext, UnsafeRawPointer?, Int) -> OSStatus

Specifies data that is sufficient to uniquely identify the peer of the current session.

Deprecated

func SSLGetPeerID(SSLContext, UnsafeMutablePointer&lt;UnsafeRawPointer?>, UnsafeMutablePointer&lt;Int>) -> OSStatus

Retrieves the current peer ID data.

Deprecated

func SSLGetSessionState(SSLContext, UnsafeMutablePointer&lt;SSLSessionState>) -> OSStatus

Retrieves the state of an SSL session.

Deprecated

enum SSLSessionState

The flags that represent the state of an SSL session.

func SSLSetError(SSLContext, OSStatus) -> OSStatus

Sets the status of a session context.

Deprecated

### Read Operations

func SSLRead(SSLContext, UnsafeMutableRawPointer, Int, UnsafeMutablePointer&lt;Int>) -> OSStatus

Performs a normal application-level read operation.

Deprecated

func SSLGetBufferedReadSize(SSLContext, UnsafeMutablePointer&lt;Int>) -> OSStatus

Determines how much data is available to be read.

Deprecated

### Write Operations

func SSLWrite(SSLContext, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;Int>) -> OSStatus

Performs a typical application-level write operation.

Deprecated

func SSLGetDatagramWriteSize(SSLContext, UnsafeMutablePointer&lt;Int>) -> OSStatus

Provides the largest packet that the OS guarantees it can send without fragmentation.

Deprecated

func SSLGetMaxDatagramRecordSize(SSLContext, UnsafeMutablePointer&lt;Int>) -> OSStatus

Obtains the maximum datagram record size allowed by the application for a given context.

Deprecated

func SSLSetMaxDatagramRecordSize(SSLContext, Int) -> OSStatus

Sets the maximum datagram record size allowed by the application for a given context.

Deprecated

func SSLSetDatagramHelloCookie(SSLContext, UnsafeRawPointer?, Int) -> OSStatus

Sets the cookie value used in the Datagram Transport Layer Security (DTLS) hello message.

Deprecated

### The Peer Domain Name

func SSLSetPeerDomainName(SSLContext, UnsafePointer&lt;CChar>?, Int) -> OSStatus

Specifies the fully qualified domain name of the peer.

Deprecated

func SSLGetPeerDomainNameLength(SSLContext, UnsafeMutablePointer&lt;Int>) -> OSStatus

Determines the length of a previously set peer domain name.

Deprecated

func SSLGetPeerDomainName(SSLContext, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Int>) -> OSStatus

Retrieves the peer domain name specified previously.

Deprecated

func SSLCopyRequestedPeerName(SSLContext, UnsafeMutablePointer&lt;CChar>, UnsafeMutablePointer&lt;Int>) -> OSStatus

Determines the buffer size needed for the peer domain name.

Deprecated

func SSLCopyRequestedPeerNameLength(SSLContext, UnsafeMutablePointer&lt;Int>) -> OSStatus

Obtains the hostname specified by the client in the ServerName extension (SNI). Server only.

Deprecated

### Versions

func SSLSetProtocolVersionMax(SSLContext, SSLProtocol) -> OSStatus

Sets the maximum protocol version allowed by the application for a given SSL context.

Deprecated

func SSLSetProtocolVersionMin(SSLContext, SSLProtocol) -> OSStatus

Sets the minimum protocol version allowed by the application for a given SSL context.

Deprecated

func SSLGetProtocolVersionMax(SSLContext, UnsafeMutablePointer&lt;SSLProtocol>) -> OSStatus

Gets the maximum protocol version allowed by the application for a given SSL context.

Deprecated

func SSLGetProtocolVersionMin(SSLContext, UnsafeMutablePointer&lt;SSLProtocol>) -> OSStatus

Gets the minimum protocol version allowed by the application for a given SSL context.

Deprecated

func SSLGetNegotiatedProtocolVersion(SSLContext, UnsafeMutablePointer&lt;SSLProtocol>) -> OSStatus

Obtains the negotiated protocol version of the active session.

Deprecated

enum tls_protocol_version_t

The collection of supported TLS and DTLS versions.

enum SSLProtocol

An enumeration of valid SSL protocol versions.

### Application Layer Protocols

func SSLCopyALPNProtocols(SSLContext, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Gets the list of supported application layer protocols.

Deprecated

func SSLSetALPNProtocols(SSLContext, CFArray) -> OSStatus

Sets the list of supported applicaiton layer protocols.

Deprecated

### Ciphers

func SSLGetNumberSupportedCiphers(SSLContext, UnsafeMutablePointer&lt;Int>) -> OSStatus

Determines the number of cipher suites supported.

Deprecated

func SSLGetSupportedCiphers(SSLContext, UnsafeMutablePointer&lt;SSLCipherSuite>, UnsafeMutablePointer&lt;Int>) -> OSStatus

Determines the values of the supported cipher suites.

Deprecated

func SSLSetEnabledCiphers(SSLContext, UnsafePointer&lt;SSLCipherSuite>, Int) -> OSStatus

Specifies a restricted set of SSL cipher suites to be enabled by the current SSL session context.

Deprecated

func SSLGetNumberEnabledCiphers(SSLContext, UnsafeMutablePointer&lt;Int>) -> OSStatus

Determines the number of cipher suites currently enabled.

Deprecated

func SSLGetEnabledCiphers(SSLContext, UnsafeMutablePointer&lt;SSLCipherSuite>, UnsafeMutablePointer&lt;Int>) -> OSStatus

Determines which SSL cipher suites are currently enabled.

Deprecated

func SSLGetNegotiatedCipher(SSLContext, UnsafeMutablePointer&lt;SSLCipherSuite>) -> OSStatus

Retrieves the cipher suite negotiated for this session.

Deprecated

func SSLSetDiffieHellmanParams(SSLContext, UnsafeRawPointer?, Int) -> OSStatus

Specifies Diffie-Hellman parameters for a given context.

Deprecated

func SSLGetDiffieHellmanParams(SSLContext, UnsafeMutablePointer&lt;UnsafeRawPointer?>, UnsafeMutablePointer&lt;Int>) -> OSStatus

Retrieves the Diffie-Hellman parameters for a given context.

Deprecated

enum tls_ciphersuite_group_t

Groups that collect ciphersuites of comparable security properties.

enum tls_ciphersuite_t

The collection of valid ciphersuites.

typealias SSLCipherSuite

A type for storing cipher suite values.

enum SSLCiphersuiteGroup

A mechanism for grouping related cipher suites.

SSL Cipher Suite Values

Recognize the set of valid SSL cipher suite values.

### Root Certificates

func SSLSetCertificateAuthorities(SSLContext, CFTypeRef, Bool) -> OSStatus

Adds one or more certificates to a server’s list of certification authorities (CAs) acceptable for client authentication.

Deprecated

func SSLCopyCertificateAuthorities(SSLContext, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the current list of certification authorities.

Deprecated

### Authentication

func SSLAddDistinguishedName(SSLContext, UnsafeRawPointer?, Int) -> OSStatus

Adds a DER-encoded distinguished name to a list of acceptable names to be specified in requests for client certificates.

Deprecated

func SSLCopyDistinguishedNames(SSLContext, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the distinguished names of acceptable certification authorities.

Deprecated

func SSLSetCertificate(SSLContext, CFArray?) -> OSStatus

Specifies this connection’s certificate or certificates.

Deprecated

func SSLGetClientCertificateState(SSLContext, UnsafeMutablePointer&lt;SSLClientCertificateState>) -> OSStatus

Retrieves the exchange status of the client certificate.

Deprecated

func SSLCopyPeerTrust(SSLContext, UnsafeMutablePointer&lt;SecTrust?>) -> OSStatus

Retrieves a trust management object for the certificate used by a session.

Deprecated

enum SSLClientCertificateState

An enumeration of the states of client certificate exchange.

func SSLSetOCSPResponse(SSLContext, CFData) -> OSStatus

Sets the OCSP response for the given SSL session.

Deprecated

func SSLSetSessionTicketsEnabled(SSLContext, Bool) -> OSStatus

Enables or disables session ticket resumption.

Deprecated

### Result Codes

Secure Transport Result Codes

Recognize result codes specific to the secure transport API.

### Legacy Operations

func SSLSetEncryptionCertificate(SSLContext, CFArray) -> OSStatus

Specifies the encryption certificates used for this connection.

Deprecated

