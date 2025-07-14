

- CFNetwork
-  Secure Sockets (SOCKS) Errors 

API Collection

# Secure Sockets (SOCKS) Errors

Error codes returned by the `kCFStreamErrorDomainSOCKS` error domain.

## Overview

Error codes in the `kCFStreamErrorDomainSOCKS` domain can come from multiple parts of the protocol stack, many of which define their own error values as part of outside specifications such as the HTTP specification.

To avoid confusion from conflicting error numbers, error codes in the `kCFStreamErrorDomainSOCKS` domain contain two parts: a subdomain, which tells which part of the protocol stack generated the error, and the error code itself.

Calling CFSocketStreamSOCKSGetErrorSubdomain(_:) returns an identifier that tells which layer of the protocol stack produced the error.

Calling CFSocketStreamSOCKSGetError(_:) returns the actual error code that the subdomain describes. This list of constants contains the possible values that this function will return. They must be interpreted within the context of the relevant error subdomain.

## Topics

### Constants

var kCFStreamErrorSOCKS4IdConflict: Int

Request rejected by the server because the client program and the `identd` daemon reported different user IDs.

var kCFStreamErrorSOCKS4IdentdFailed: Int

Request rejected by the server because it couldn’t connect to the `identd` daemon on the client.

var kCFStreamErrorSOCKS4RequestFailed: Int

Request rejected by the server or request failed.

var kCFStreamErrorSOCKS4SubDomainResponse: Int

The SOCKS4 status code returned by the server.

var kCFStreamErrorSOCKS5SubDomainMethod: Int

The server’s desired negotiation method.

var kCFStreamErrorSOCKS5SubDomainResponse: Int

The response code that the server returned in reply to the connection request.

var kCFStreamErrorSOCKS5SubDomainUserPass: Int

The status code that the server returned during authentication.

var kCFStreamErrorSOCKSSubDomainNone: Int

A general SOCKS error.

var kCFStreamErrorSOCKSSubDomainVersionCode: Int

The version of SOCKS that the server wants to use.

var kSOCKS5NoAcceptableMethod: Int

The client and server couldn’t find a mutually agreeable authentication method.

var kCFStreamErrorSOCKS5BadResponseAddr: Int

The address returned is not of a known type. This error code is only valid for errors in the `kCFStreamErrorSOCKSSubDomainNone` subdomain.

var kCFStreamErrorSOCKS5BadState: Int

The stream is not in a state that allows the requested operation. This error code is only valid for errors in the `kCFStreamErrorSOCKSSubDomainNone` subdomain..

var kCFStreamErrorSOCKSUnknownClientVersion: Int

The SOCKS server rejected access because it does not support connections with the requested SOCKS version. SOCKS client version. You can query the `kCFSOCKSVersionKey` key to find out what version the server requested. This error code is only valid for errors in the `kCFStreamErrorSOCKSSubDomainNone` subdomain.

## See Also

### Streams

func CFReadStreamCreateForHTTPRequest(CFAllocator?, CFHTTPMessage) -> Unmanaged&lt;CFReadStream>

Creates a read stream for a CFHTTP request message.

Deprecated

func CFReadStreamCreateForStreamedHTTPRequest(CFAllocator?, CFHTTPMessage, CFReadStream) -> Unmanaged&lt;CFReadStream>

Creates a read stream for a CFHTTP request message object whose body is too long to keep in memory.

Deprecated

let kCFStreamPropertyHTTPAttemptPersistentConnection: CFStringDeprecated

let kCFStreamPropertyHTTPFinalRequest: CFString

HTTP Final Request property. A value of type CFHTTPMessage containing the final message transmitted by the stream after all modifications (including authentication, connection policy, redirects, and so on) have been made. This property cannot be set.

Deprecated

let kCFStreamPropertyHTTPFinalURL: CFString

HTTP Final URL property. A value of type CFURL containing the final HTTP URL. This value differs from the URL in the original HTTP request if an autoredirection occurred. This property cannot be set.

Deprecated

let kCFStreamPropertyHTTPProxy: CFStringDeprecated

let kCFStreamPropertyHTTPProxyHost: CFStringDeprecated

let kCFStreamPropertyHTTPProxyPort: CFStringDeprecated

let kCFStreamPropertyHTTPRequestBytesWrittenCount: CFStringDeprecated

let kCFStreamPropertyHTTPResponseHeader: CFString

HTTP Response Header property. When copied by CFReadStreamCopyProperty(_:_:), the header of an HTTP response message is returned.

Deprecated

let kCFStreamPropertyHTTPSProxyHost: CFStringDeprecated

let kCFStreamPropertyHTTPSProxyPort: CFStringDeprecated

let kCFStreamPropertyHTTPShouldAutoredirect: CFString

HTTP Should Auto Redirect property. Set this property to `kCFBooleanTrue` to enable autoredirection; set this property to `kCFBooleanFalse` to disable autoredirection.

Deprecated

func CFWriteStreamCreateWithFTPURL(CFAllocator?, CFURL) -> Unmanaged&lt;CFWriteStream>

Creates an FTP write stream.

Deprecated

func CFReadStreamCreateWithFTPURL(CFAllocator?, CFURL) -> Unmanaged&lt;CFReadStream>

Creates an FTP read stream.

Deprecated

